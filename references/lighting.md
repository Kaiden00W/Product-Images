# Exposure, Background, Grounding and Lighting

The half of the job that decides whether it looks like a product photograph or a
render. White parts are the hard case — this is where most of the failures live.

---

## EXPOSURE — THE MOST COMMON FAILURE ON WHITE PARTS

White powder coat clips easily, and once it clips you lose the panel's form, the
grain, and the edge definition. "Slightly under-expose" is too soft to act on.

```
EXPOSURE — THIS IS THE MOST IMPORTANT SETTING. Expose for the white part, not the
background, and expose it CONSERVATIVELY. The most common failure on this part is
over-exposure.
• NO pixel on the part reaches pure white. The brightest white surface sits at roughly
  80% brightness, leaving clear headroom at the top. Even the lightest, most directly lit
  plane is visibly a light grey-white, not paper white.
• THE PLASTIC TEST: the textured powder-coat micro-grain must be clearly visible on EVERY
  surface, including the brightest upper-facing planes. If any panel looks like smooth
  plastic, vinyl or moulded polymer, it is over-exposed — bring it down until the grain
  returns.
• Each folded facet sits at a visibly different brightness from its neighbours, so the
  geometry reads as distinct planes rather than one bright mass. Shaded sides go
  meaningfully darker.
• Every edge stays crisp. No clipped highlights, no blown-out flat areas, no glow,
  halation or bloom, no soft or fuzzy contours.
If in doubt, expose darker.
```

**Dial:** if still hot, change `80%` → `75%`. Change the number, not the words.

⚠️ **Words like "cinematic", "premium", "hero shot" and "high-key" all push brightness
up.** If you use them, counterweight explicitly:

```
Cinematic lighting means MORE tonal range, never more brightness — the drama comes from
deeper shadows, not hotter highlights.
```

If a part keeps blowing out, **remove the aspirational adjectives before adding more
exposure rules.** They are usually the cause.

---

## BACKGROUNDS

### Pure white (default for black parts)
```
BACKGROUND: a plain, solid, pure white background — completely empty and featureless. No
studio, softbox, light tent, diffusion panels, walls, corners, seams, floor line or props.
Genuinely white and evenly lit — not grey, dim, gradient-shaded or vignetted. Clean white
shows through every slot, hole and cut-out.
```

### Grey (required for white or light parts)
A white part on white has no separation. Grey values that worked:

| Situation | Value |
|---|---|
| All-white part | `#6B6B6B` — mid-dark, strong separation |
| Two-tone part with a black component | `#7A7A7A` – `#828282` — light enough that the black reads too |

```
BACKGROUND: a neutral grey seamless studio backdrop around #6B6B6B, no blue, green or warm
cast, no texture, walls, corners, seams or props.

Give it a SMOOTH, DELIBERATE GRADIENT rather than a flat field: softly lifted BEHIND and
ABOVE the part in the upper middle of the frame, falling off gently darker toward the frame
edges and upper corners. The falloff must be perfectly smooth and continuous — no banding,
no blotches, no patchy areas, no hard-edged pool of light, and NO bright halo or glowing
ring outlining the part. The gradient belongs to the backdrop as a whole, not to the shape
of the product sitting on it.
```

⚠️ A flat grey field is technically clean but visually inert. A *controlled* gradient is
what reads premium. The distinction is **intentional and smooth** vs **accidental and
patchy** — say both.

---

## GROUNDING — THE SECOND MOST COMMON FAILURE

Parts float. The cause is almost always brightening the area *underneath* them, or a
floor reflection that overpowers the contact shadow.

```
THE FLOOR AREA IS THE DARKEST PART OF THE BACKDROP. The surface immediately beneath and
around the base of the part is noticeably DARKER than the backdrop behind it, and darkens
further as it approaches the part. Never brighten the area under the part — that is what
makes a product look like it is floating.

GROUNDING — THE PART MUST SIT ON THE SURFACE, NOT HOVER. At EVERY point where the part
touches down, render a firm CONTACT SHADOW with a genuinely DARK, TIGHT CORE right at the
point of contact, spreading and softening outward. No gap, no glow and no light leak
between the metal and the ground at any contact point.

The surface has only the faintest sheen — a very subtle, short, low-contrast reflection
directly beneath the part, fading almost immediately. Never mirror-like, never sharp, and
never brighter or more prominent than the contact shadow. If the reflection competes with
the shadow, reduce the reflection: the shadow grounds the part, the reflection is only a
hint of surface.
```

⚠️ **Never write "lifted behind and just below the part".** The lift *below* is precisely
what destroys grounding.

---

## LIGHTING

### Clean catalogue (default, black parts on white)
```
LIGHTING: bright, clean, high-key product lighting that reaches every recessed, concave and
interior face with no muddy dark pockets, while keeping real tonal separation between
facets so each folded plane sits at a different brightness and the geometry reads strongly
three-dimensional. Deep blacks in the shadowed planes, clean highlights on the up-facing
planes, a crisp specular line on every fold.
```

### Cinematic (hero shots, grey backdrop)
```
LIGHTING — DIRECTIONAL AND SCULPTED. Not flat, not evenly washed, not a spec-sheet setup:
• A large soft KEY LIGHT from the upper front-left at about 45 degrees, establishing a
  clear lit side and a clear shadowed side. Committed direction.
• A gentler FILL from the opposite side at roughly a third of the key's strength, so
  shadowed planes stay readable with detail but remain unmistakably darker. Never lift the
  shadows to match the key.
• A crisp RIM / KICKER from behind and above, skimming the top edges and the far
  silhouette. This is the most important element — without it a white or light part
  dissolves into the grey behind it.
• Crisp specular lines catch every folded edge and cut edge.
```

**The rim light is the single biggest upgrade for a light part on a grey backdrop.**

**Dial:** too moody for a product listing → raise fill from a third of key to a half.
Leave the rim alone.

---

## COMPOSITION

```
COMPOSITION — A CROP, NEVER A RE-SHOOT: you may present the part larger in frame than the
source does, but this is a PURE CROP AND ZOOM of the identical photograph, like enlarging
a print. The camera does not move and NO NEW SURFACE BECOMES VISIBLE. If making it bigger
would require seeing more of the part, do not make it bigger. Matching the source angle
always beats filling the frame. Centre it with even margins, cropping nothing off.
```

⚠️ Never write a bare "fill most of the frame with even margins" alongside a camera lock.
That exact pair made a skid plate re-shoot itself from a higher angle.

---

## RENDER QUALITY

```
RENDER QUALITY: photoreal, physically accurate materials, tack sharp with crisp
well-defined edges, rich tonal contrast with deep true blacks and clean bright highlights,
neutral true-to-life colour, subtle film grain, gentle highlight rolloff. Indistinguishable
from a real high-end studio product photograph.
```

Include this on **every** prompt including small edits — the model re-renders the whole
frame, so anything not restated is at risk of degrading.
