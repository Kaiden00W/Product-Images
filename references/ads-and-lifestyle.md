# Ads, Hero Images and Lifestyle Creative

Creative mode. The subject is a scene that sells something, not a part being
transcribed. Different instincts apply — but the same discipline about
contradictions and length.

**Target length: 800–2,000 characters.** Ad prompts fail from bloat faster than
fidelity prompts do. If it's over 2,000 you're probably over-specifying.

---

## THE SHAPE OF A GOOD AD PROMPT

Write it as a brief to a photographer, not a keyword list.

```
[Shot type] of [specific subject with real detail] [action] at [specific location],
[time of day and light], [mood], [camera and lens feel], [colour direction].
[What it's for.]
```

Everything that follows is a way of making one of those slots specific.

### Say what it's FOR
Stating the use case pulls in a whole set of sensible defaults — lighting,
composition, energy — without you specifying each one.

> "Shot for a jet ski rental company's summer Google Display campaign."
> "Hero banner for a performance mechanic shop's website."

### Be specific about the subject
"A jet ski on a lake" gets you stock. Specify make/colour/state, who's on it, what
they're doing, what the water is doing.

> Weak: *two people on a jet ski*
> Strong: *two friends in their late twenties on a red-and-white three-seat
> waverunner, mid-turn and throwing a wide arc of spray, both laughing, life
> jackets on*

### Name the real place
Local specificity beats generic scenery, and it's free.

> *Okanagan Lake with the dry sagebrush hills of the Naramata bench behind them,
> late afternoon in July*

### Direct the light explicitly
The single biggest driver of whether it reads premium or stock.

> *golden hour, low warm sun raking across the water from behind them, backlit spray
> catching the light, long soft shadows*

### Camera language
> *wide establishing shot* · *tight three-quarter* · *low angle from water level*
> *shallow depth of field* · *shot on a 70-200mm at 200mm, compressed background*
> *slight motion blur in the spray, subject sharp*

---

## THE THINGS THAT GO WRONG IN ADS

### Invented text and signage
The number one giveaway. Models scatter garbled lettering across signs, boats,
buildings and clothing.

```
No text, signage, lettering, logos, brand marks, numbers or watermarks anywhere in
the image.
```

If you need real text, **add it in afterwards** in a design tool. Generated text is
unreliable at small sizes and unusable at any size in a regulated ad.

### People
Hands, faces, and repeated faces across a campaign are the hard parts.

```
Natural, candid expressions — genuinely mid-action, not posed for camera. Correct
anatomy with clearly formed hands. Real skin texture, not airbrushed.
```

- For a **consistent person across several images**, use a reference photo and say
  *"keep the facial features exactly consistent with the reference"*.
- If faces keep failing, **turn them away** — over the shoulder, mid-action, backlit
  silhouette, helmet or sunglasses on. Often better creative anyway.

### Uncanny product details
If a real product appears in the shot, that part is **fidelity mode**. Give it a
locked block at the top of the prompt and treat the rest as creative:

```
RULE ZERO — [PRODUCT] FIDELITY: reproduce the [product] exactly as the reference
shows it. Same shape, proportions, colour, graphics and detailing. Do not restyle,
simplify or redesign it. Everything else in the scene is yours to compose.
```

### Real logos
Same principle — **fidelity block, front-loaded**, because the model will otherwise
"improve" kerning and letterforms.

```
RULE ZERO — LOGO FIDELITY. The uploaded logo is a FIDELITY reference, not a style
reference. Reproduce it EXACTLY as supplied — same glyph shapes, stroke weights,
slant, letter spacing and kerning. Copy the letterforms; do not redraw them, do not
"improve" or re-balance the kerning, do not substitute a similar font. Same colours,
same internal proportions. Add no word, tagline, or graphic element that is not in
the supplied file, and remove nothing.
```

And make it obey the surface it sits on:
```
The decal sits ON the surface, not floating above it: it wraps and undulates with
the surface contour, takes the same directional light and falloff as the material
around it, and has a slight sheen difference from the substrate. Subtle authentic
micro-wear only — fully legible and clearly intact.
```

**Realistic expectation:** a detailed logo reproduced onto a textured, unevenly lit
surface is one of the hardest things to get. If it keeps degrading, generate the
scene **without** the logo and composite the real artwork in afterwards — with a
multiply pass for surface shadows and a soft mask carrying the scene's light falloff.

---

## BRAND COLOUR DISCIPLINE

If the business has a palette, lock it — otherwise the model adds teal and magenta.

```
[BRAND COLOUR] #XXXXXX IS THE ONLY SATURATED COLOUR IN THE IMAGE. Everything else is
near-black, charcoal, cool grey, desaturated blue-grey or sparing white. No teal, no
cyan, no magenta, no purple, no secondary coloured light sources anywhere.
```

Fence the hero colour from both sides so it can't drift:
> *vivid saturated signal red, approximately RAL 3020 (~#CC1611) — not orange,
> vermilion, coral or scarlet; not pink, maroon, burgundy or crimson*

---

## FORMATS AND SAFE AREAS

If copy or a logo overlays the image, reserve space **in the prompt** — retrofitting
is painful.

```
Keep the top ~15% and the bottom third visually CALM — smooth, low-detail,
low-contrast, free of clutter and busy texture, carrying only soft tonal gradients.
Headline copy and a logo overlay those zones and must stay readable. Detail and
interest live in the middle band.
```

**Common ad ratios** — generate the ratio you need rather than cropping later, since
composition changes with the frame:

| Placement | Ratio |
|---|---|
| Google Display — landscape | 1.91:1 |
| Google Display — square | 1:1 |
| Website hero | 16:9 |
| Social feed | 4:5 or 1:1 |
| Stories / Reels / Shorts | 9:16 |

**Generate portrait separately.** Cropping a 16:9 to 9:16 destroys the composition —
prompt it fresh with the subject recomposed for the tall frame.

---

## STYLE REFERENCE IMAGES

Borrowing a look from a reference is powerful and leaks badly if unscoped:

```
IMAGE 2 is a STYLE reference only. Borrow its lighting, colour grade, materiality
and camera discipline. Take NOTHING else from it — not its subject, not its
composition, not its logo, signage or text, not its resolution or softness. Do not
reproduce any element of it as content.
```

---

## WORKED EXAMPLE — jet ski rental, Google Display

```
A wide, low-angle action photograph taken from water level: two friends in their late
twenties riding a red-and-white three-seat waverunner, mid-turn and throwing a broad
arc of spray toward camera, both laughing, life jackets on. Okanagan Lake in
mid-July, the dry sagebrush hills of the Naramata bench rising behind them, a few
other boats small and distant on the water.

Golden hour: low warm sun raking in from behind them, backlighting the spray so it
glows, long soft shadows, deep blue-green water with sun glitter. Warm, energetic,
genuinely fun — a real summer afternoon, not a staged advert.

Shot on a full-frame body at 200mm, compressed background, shallow depth of field,
subject tack sharp with slight motion blur in the flying spray. Rich natural colour,
clean highlights, subtle film grain.

Keep the top 15% and the bottom third calm and uncluttered for headline copy and a
logo overlay.

Photoreal, indistinguishable from a real photograph. No text, signage, lettering,
logos, brand marks or watermarks anywhere. Natural candid expressions with correct
anatomy and clearly formed hands.

1.91:1 landscape, high resolution.
```

~1,200 characters. Note what it does **not** do: no keyword soup, no "8k masterpiece
trending on artstation", no list of camera brands. Specific subject, specific place,
specific light, stated purpose, and the two guardrails that actually matter for ads
— no invented text, and safe areas reserved.
