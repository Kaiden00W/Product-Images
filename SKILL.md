---
name: product-image-prompts
description: >-
  Write prompts for AI image and video generation — Nano Banana Pro, Kling, Veo,
  Seedance, Higgsfield and similar. Covers two modes: FIDELITY work (turning CAD
  renders into product photos, recolouring products, reproducing a logo exactly) and
  CREATIVE work (ads, hero images, lifestyle and marketing imagery, short video).
  Use when the user mentions Nano Banana, NBP, Kling, an image or video prompt, a CAD
  render, a product photo, a recolour, an ad creative, a hero image, or a marketing
  visual. Also use when a generation came back wrong and needs diagnosing.
---

# Image & Video Prompting

Built from several hundred real iterations across product photography, brand hero
images, logo work and scroll-driven video. Every rule here exists because something
failed without it.

---

## FIRST: WHICH MODE?

The two jobs need opposite instincts. Decide before writing a word.

| | **FIDELITY MODE** | **CREATIVE MODE** |
|---|---|---|
| Job | Reproduce something exactly | Generate a scene that sells something |
| Examples | CAD → product photo, recolouring a part, placing a real logo | Ads, hero images, lifestyle shots, social creative |
| The enemy | Invention — added bolts, invented symmetry, re-framed camera | Blandness, stock-photo feel, uncanny people |
| Prompt shape | Constraints and freezes | Direction, mood, specificity |
| Length | 3,000–6,000 chars | 800–2,000 chars |
| Reference images | Essential — geometry the model can't guess | Optional — style or brand anchors |

Mixed jobs exist: an ad containing a real product or logo. Then the **fidelity part
gets a locked block at the very top** and the rest of the prompt is creative.

---

## RULES THAT APPLY TO BOTH

### 1. Start short. Stay short.
Google's own guidance lists over-prompting as an anti-pattern, and it holds up: a 10k
prompt beat the 13.6k version of itself, and a 3.2k rewrite beat both. Long prompts
fail because critical rules end up competing with paragraphs about softboxes.

**Cut a working section before adding a new rule.**

### 2. Fix the wrong line. Never stack a counter-rule.
The biggest cause of failure is prompts that argue with themselves:

| Instruction written | What it caused |
|---|---|
| "fill most of the frame" + "the camera is locked" | Subject re-shot from a new angle |
| "clean, neutral, **slightly warm** white" | Came out cream |
| "NO shaft protruding either way" | Deleted a bolt thread the user wanted |
| "EXACTLY THREE weld nuts" reused on a different part | Converted three cut-outs into three nuts to hit the quota |
| "cinematic", "premium", "hero shot" | Pushed exposure until the subject blew out |

When something fails, find the line that caused it and change **that line**.

### 3. Numeric ceilings and functional tests beat adjectives.
"Small" and "don't over-do it" never worked. These did:

- **Ratio:** "each nut is roughly 1/30th of the plate's length"
- **Absolute:** "M8, about 13mm across the flats" / "roughly #6B6B6B"
- **Functional:** "if it reads as a prominent feature, it's too big"
- **Functional:** "if any panel looks like smooth plastic, it's over-exposed"
- **Functional:** "if you can see a surface that wasn't visible in the source, the camera moved"

The model can check these. It cannot check "small".

### 4. Show, don't describe.
**The highest-leverage tool available.** Twice a reference image fixed in one pass what
three rounds of prose could not. NBP Pro takes **up to 14 reference images, 6 at high
fidelity**. Use them.

Always scope them or the output drifts toward their framing:
> IMAGE 1 IS THE SHOT — camera, viewpoint, perspective and framing all come from it.
> ALL OTHER IMAGES ARE REFERENCES. Take nothing else from them: not their angle,
> framing, scale, lighting or colour.

### 5. Inverting a default overshoots unless you state the target.
- "don't over-weld" → "start at zero, earn each bead" → **nothing got welded**
- → "fill every gap, no ceiling" → **beads on every fold line**
- correct: "every gap between two separate panels is welded shut; a fold is not a gap"

Always pair the suppression with the correct amount.

### 6. Audit as a hunt, not a confirmation.
"Scan for anything still black" catches more than "confirm everything is orange."

---

## PRE-FLIGHT — BEFORE SENDING ANY PROMPT

1. Does any instruction contradict another? (freeze rules vs composition; colour vs colour)
2. Is every hard-coded count/fact true for **this** subject, checked against the source?
3. Does any new rule damage something it shouldn't touch?
4. Is it within the length band for its mode, and did you cut before you added?
5. Could a reference image replace a paragraph of description?
6. **Video models with a negative field:** does any negative term appear as a wanted
   noun in the positive? ("zoom during the door opening" suppressed *door opening*.)

---

## REFERENCE FILES

**Fidelity mode**
- `references/cad-to-photo.md` — CAD → photoreal product photograph; the hardware,
  weld and camera rule sets that took longest to get right
- `references/recolour.md` — colour changes on existing renders, two-tone splits,
  brand colour specs

**Creative mode**
- `references/ads-and-lifestyle.md` — ads, hero images, lifestyle and location
  shoots, people, real logos in scenes, text and safe areas, ad formats

**Both**
- `references/lighting.md` — exposure, backgrounds, grounding, cinematic lighting
- `references/video.md` — Kling and other video models: timing beats, negative
  prompts, keyframes, camera locks

---

## WORKFLOW

1. Establish the mode. Ask what the source is and what the output is for.
2. **Fidelity:** ask for every reference view they have. Biggest quality lever.
   **Creative:** ask where it runs (Google Display, social, hero banner) — the
   format and safe areas change the prompt.
3. Pull the matching template, fill it from the source in front of you. Never carry
   subject-specific facts or counts across from a previous job.
4. Run the pre-flight.
5. Deliver in a copy-paste block with its character count.
6. When it comes back wrong, diagnose from the image and fix the **one line**
   responsible.
