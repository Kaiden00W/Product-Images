# Recolouring an Existing Product Photo

Input is a finished render, not a CAD. The job is to change colour and nothing else.

**Critical model behaviour:** NBP does not do local edits — it **re-renders the whole
frame every time**. So a short "just change the colour" prompt strips out every quality
instruction the good render depended on, and the result degrades (texture flattens to
vinyl, welds go soft, background greys out). **Every recolour prompt must carry a
compact material and quality spec**, even when the edit is tiny.

---

## THE UNIVERSAL SPINE

Every recolour prompt uses this skeleton:

1. **What turns [colour]** — enumerate the components, including weld beads
2. **The colour spec** — hex + fenced on both sides
3. **What stays as it is** — hardware, and any second colour
4. **Surface finish** — preserve or change, stated explicitly
5. **Freeze block** — geometry, hardware count, welds, camera, lighting, background
6. **Render quality**
7. **Final check** — as a *hunt* for the wrong colour, not a confirmation

---

## COLOUR SPECS THAT WORKED

| Colour | Spec | Fence against |
|---|---|---|
| Signal red | RAL 3020, ~`#CC1611` | orange, vermilion, coral, scarlet, tomato / pink, maroon, burgundy, crimson |
| KTM racing orange | RAL 2004, ~`#F35B04` | yellow, amber, gold, tan, peach / red, scarlet, brown, rust |
| White | pure neutral white | cream, ivory, beige, off-white, warm-white, blue-white, grey |

⚠️ **Never write a self-contradictory colour phrase.** "clean, neutral, *slightly warm*
architectural white" produced cream. Fence from both directions, never hedge in the middle.

---

## THE THREE HARD-WON RULES

### 1. A clamp is TWO components at one spot
The most repeated failure across every colour.

```
A clamp is TWO things at one spot: the collar BODY is [colour] textured powder coat; its
BOLTS, NUTS and WASHERS are polished stainless steel. Do not let the coating flow over its
own hardware. [Colour] body, bright silver bolts, on every clamp on the part.
```

### 2. Hardware is defined in BOTH directions
A one-way shape test ("anything shaped like a hex head is a fastener") swept clamp
collars into the stainless bucket and rendered them chrome.

```
A FASTENER, rendered polished stainless, is ONLY one of four things: a HEX BOLT HEAD, a
HEX NUT, a WASHER, or a length of EXPOSED THREADED SHAFT.

NOT FASTENERS — structural, and PAINTED: clamp collars, collar bodies, saddles, bands,
straps, clips, brackets, gussets, tabs, plates, lugs, mounts and spacers. Painted no
matter that they are metal fittings, no matter that they have bolts through them.

If a component is bigger than a nut and is not itself threaded, it is painted.
```

### 3. Interiors and shadows keep the colour
Bores and recesses render as black voids otherwise.

```
INSIDES COUNT: the bore of every clamp collar and every open tube end is [COLOUR] PAINTED
METAL — [colour] receding into shadow, NOT a black hole, black void or dark plug.

[COLOUR] SHADOWS STAY [COLOUR]: deep shadow becomes a deeper, richer, more saturated
[colour] — never grey, charcoal or black.

There are NO black rubber or plastic parts anywhere — no bushings, grommets, sleeves,
inserts, caps or end plugs. Anything reading as a black insert is painted metal.
```

---

## TWO-TONE SPLITS

The boundary is **welded vs bolted**, not tube vs sheet — small tabs welded to tubes
are body-colour even though they are flat sheet.

```
[COLOUR] — THE TUBULAR FRAME: every round tube; every clamp collar body; every small flat
MOUNTING TAB or lug WELDED onto a tube (body-colour even though it is flat sheet, because
it belongs to the frame); every weld bead on the frame.

BLACK — THE BOLT-ON FLAT BRACKETRY: the tall flat vertical CENTRE BRACKET and the flat
horizontal CROSSBAR STRAP that bolt to the [colour] welded tabs. [Add the skid plate here
for a combo.]

Nothing else is black. To be unambiguous, everything in this list is [COLOUR]: the tall
upright mounting brackets with bolt holes, the triangular gussets, the clamp collars, the
tube end caps and spacers, and the small end tabs on the top strap. Do not leave any
additional component black, and do not turn any extra bracket black for visual balance.

CRISP BOUNDARIES: where black meets [colour], a clean sharp edge at the physical join. No
bleeding, feathering or gradient either way.
```

**Fence the exception from both sides.** Listing only what stays black lets the black
spread; listing what must NOT be black is what stopped it.

---

## FINISH: PRESERVE OR CHANGE — SAY WHICH

```
PRESERVE (default):
Keep the identical TEXTURED powder-coat surface: the same fine sandy micro-grain, the same
low gloss, the same soft broad highlights. Only the pigment changes. Do NOT convert to
smooth gloss, wet-look, candy, metallic, pearl or clearcoat.

CHANGE TO GLOSS:
The surface changes finish as well as colour: from textured matte to SMOOTH HIGH-GLOSS
powder coat, roughly 85-90 gloss units. Wipe the texture off completely. A crisp, bright,
TIGHT specular highlight ribbon runs along the crown of each tube — narrow and hard-edged,
not a soft broad wash. This tight highlight is what makes the gloss read. NO mirrored
surroundings: the environment is empty white, so the gloss shows clean highlights and
smooth falloff only, never a reflected scene.
```

---

## WELD BEADS UNDER PAINT

```
Every existing weld bead keeps its raised, rippled stack-of-dimes relief, clearly readable
as a raised ridge of metal beneath the [colour] — catching the light along each ripple. Do
NOT smooth, melt, flatten, fill, blur or erase any weld bead.
```

Gloss finishes and colour changes both tend to soften weld relief. Always include this.

---

## THE FREEZE BLOCK

```
CHANGE NOTHING ELSE.
• HARDWARE COUNT IS FROZEN. Add no bolt, nut or washer anywhere. Remove, move, resize or
  restyle none that are present.
• GEOMETRY IS FROZEN. Every tube, bend, curve, junction, bracket, tab, plate and hole stays
  exactly where and as it is. Add nothing, remove nothing, reshape nothing, and do NOT
  mirror or duplicate any component.
• WELDS ARE FROZEN. Every bead stays where it is, at the same size and relief.
• CAMERA IS FROZEN. Identical angle, viewpoint, perspective, framing, crop, and subject size
  and position in frame. No surface may become visible that was not visible already.
• LIGHTING IS FROZEN. Identical light directions and highlight placement.
• BACKGROUND IS FROZEN. Same background and contact shadow.
```

---

## THE FINAL CHECK — HUNT, DON'T CONFIRM

```
FINAL CHECK — scan the ENTIRE part for anything still [old colour]. The only permitted
non-[new colour] objects are the silver threaded fasteners. Recolour anything else.
Look specifically INSIDE every clamp bore and open tube end. Look at every recess, notch
and inner corner. Confirm no black rubber or plastic insert remains anywhere.
```

---

## USING A REFERENCE IMAGE FOR THE COLOUR SPLIT

When the user has a mock-up of the target scheme, this beats any amount of prose:

```
IMAGE 1 is THE PART. Everything about the photograph comes from here: geometry, camera
angle, framing, lighting, shadow, background, resolution and surface texture.

IMAGE 2 is THE COLOUR MAP, and nothing else. Use it ONLY to see WHICH COMPONENTS ARE
[COLOUR A] AND WHICH ARE [COLOUR B]. Copy that split exactly.

Take NOTHING else from image 2 — not its camera angle, framing, lighting, resolution,
softness, compression, background, or any edge artefact in it. It is a paint chart, not a
photograph to imitate.
```
