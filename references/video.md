# Video Prompts — Kling, Veo, Seedance, Hailuo

Video prompts are **much shorter** than image prompts and the craft is different.
Most models cap the prompt field around 2,000–2,500 characters, and past that
attention dilutes and you get *less* control, not more.

---

## THE FIELD BUDGET

| Field | Target |
|---|---|
| Positive prompt | 1,200–1,800 chars |
| Negative prompt | 500–750 chars |
| Combined (single-box UIs) | under 2,000 |

Density, not length. Everything defensive goes in the **negative** field, where it
belongs — not buried in the positive.

---

## TIMING BEATS — THE BIGGEST SINGLE TECHNIQUE

Video models weight temporal structure heavily. Break the clip into labelled windows:

```
0-1.5s: Locked tripod, completely still. [Establishing state.]

1.5-4s: [The main action begins, with a specific physical detail.] The camera does
not move at all.

4-5.5s: [The action completes and settles.] The camera is still locked.

5.5-9s: [Second phase — camera move, if any.]

9-11s: [Resolution.]

11-12s: The camera decelerates and stops. Everything still.
```

Beats buy you three things a flat description can't:
- **a half-second of stillness at the head** so the clip doesn't lurch on frame one
- **an ease-out at the tail** so the final frame is clean (essential if you're
  grabbing it as a keyframe for the next shot)
- **a defined moment for a specific physical event** — the jolt as a shutter breaks
  free, the instant a spray of water launches

Restate camera state **inside** each beat, not only in a summary line at the end.
A lock stated next to the action it constrains binds far better.

---

## NEGATIVE PROMPTS

Negatives are embedding-based, not sentence-parsed. Consequences:

**⚠️ Never put a wanted noun in the negative.**
- `"zoom during the door opening"` → suppressed *door opening*
- `"headlights"` on a shot that had to reveal a car → fought the end keyframe

**⚠️ Negatives cannot encode timing.** `"early camera movement"` does nothing.
Timing belongs in the positive beats.

**Order matters** — lead with the failure most likely for this shot.

Working negative for a locked-off plate:
```
camera drift, pan, tilt, roll, arc, orbit, curved path, drifting sideways, handheld,
shake, jitter, digital zoom, crop zoom, deforming geometry, melting, morphing,
shifting walls, jump cut, scene change, fade to black, changing text, garbled
writing, people, person, blurry, low quality, watermark, text overlay, cartoon,
3d render, cgi
```

Add per shot: `bending slats, warping metal, rubbery [object]` for rigid mechanical
motion · `car moving, wheels turning, duplicate car` for a static hero object ·
`purple, violet, magenta, cyan, rainbow lighting` to hold a brand palette.

---

## KEYFRAMES (start + end frame)

Supported by Kling, Runway Gen-4 and Luma. It's how you control where a clip lands.

**Check the geometry is actually continuous first.** Two frames that aren't
reachable by one camera move will morph. Signs of a discontinuity: the subject
framed by something in frame A that's absent in frame B means the camera travelled
*through* it — that's two shots, not one.

**Splitting into two shots is usually the better edit anyway:**
1. Shot 1: start frame only, action happens, camera locked, ~5s
2. Grab the last frame: `ffmpeg -sseof -0.1 -i shot1.mp4 -vsync 0 -q:v 2 -update 1 last.png`
3. Shot 2: that frame as start, your target as end, ~5s
4. Concatenate — the cut is invisible because shot 2 begins on shot 1's exact last frame

**Hiding a mismatch:** if the intermediate state can't be predicted, obscure it.
Haze, smoke, a light coming up, or a foreground element passing through covers the
transition and reads as intentional. Prompting *"the interior stays dark and
unresolved"* in shot 1 stops the model inventing detail that shot 2 then contradicts.

**Camera preset: set it to Static/None even for a move**, when both keyframes are
set. A built-in dolly preset fights the interpolation and produces a curved,
overshooting move. The keyframes already define the travel.

---

## CAMERA CONTROL LANGUAGE

**To lock:**
```
Locked-off tripod. The camera does not move at all — no push in, no pull back, no
pan, tilt, drift, zoom or handheld shake. The frame is completely static and only
[the subject] changes.
```

**For real travel rather than a crop-in:**
```
The camera physically travels forward, dead straight along the centre axis with real
parallax. The vanishing point stays locked at the centre of the frame throughout.
```
Pair with `digital zoom, crop zoom` in the negative. Parallax is what separates a
walk-in from a punch-in.

**Elements that must leave frame** — name them, or they smear at the edge:
```
The [sign] and the [wall lights] drift outward and pass out of frame as the camera
advances.
```

**Continuity on a multi-phase clip:**
```
One continuous take, no cuts.
```
Put it as the **first line**. Models weight the opening heavily and a 10s clip with
two distinct phases will otherwise insert a cut.

---

## MODEL NOTES

| Model | Use for | Watch |
|---|---|---|
| **Kling** (3.0 / 2.x) | Default. Best keyframe interpolation; best rigid-body/mechanical motion | Audio generation may be on by default — turn it off for muted web video |
| **Kling Motion Control** | When the camera keeps drifting despite instructions — lock camera, brush motion onto one region only | Lower max resolution |
| **Runway Gen-4** | Backup for keyframes; clean camera moves | Weaker on rigid-body physics |
| **Hailuo / MiniMax** | High-dynamic organic motion | Poor for locked-off mechanical shots |
| **Seedance** | General backup with first/last frame | — |

**Rigid mechanical motion is the hardest thing to get.** Expect 4–8 attempts on a
rolling shutter, a mechanism, a door. Failure modes: rigid parts bending like fabric,
the object sliding sideways, the camera drifting despite the lock.

**Escape hatch:** if a mechanical motion won't land after ~8 tries, stop paying for
generations and do it in CSS or After Effects — a `clip-path` animation over a static
image is perfectly rigid and often *is* the motion you wanted.

---

## SETTINGS

```
Duration:  5s per shot (10-12s total is plenty; longer scroll videos feel endless)
Aspect:    16:9 for web hero; generate 9:16 separately for mobile, never crop
Resolution: highest available — downscaling is cleaner than upscaling later
Audio:     off for muted web video
CFG/Relevance: 0.6-0.7 — higher over-follows the text and distorts the plate;
           lower and the negatives stop biting
```

---

## POST

Conform before building anything downstream — generated files often come back at odd
dimensions with an unwanted audio track:

```bash
ffmpeg -i in.mp4 -an -vf "scale=1920:1080:flags=lanczos" -c:v libx264 \
  -crf 16 -pix_fmt yuv420p master.mp4
```

**Scroll-scrubbed video on a website:** encode as an image sequence on a canvas
(~150 WebP frames at 1600px ≈ 5–7MB) rather than scrubbing a `<video>` element.
Video scrubbing is unreliable on iOS Safari; an image sequence is what Apple uses.
Always honour `prefers-reduced-motion` with a static frame.
