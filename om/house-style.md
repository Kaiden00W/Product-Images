# OM House Style

The constants that repeat across every Outback Motortek prompt. When you write or adapt a prompt,
take these blocks **word for word**. Each phrase is here because a looser version failed.

---

## Finishes

| Finish | Spec as written in the prompts | Used for |
|---|---|---|
| **Standard black** | Textured black powder coat, fine even sandy micro-grain, low gloss **~15 gloss units**, soft broad highlights, deep rich neutral black, **no blue or brown cast**. The grain must read as real powder coat, not a smooth 3D surface. | Every product by default |
| **Signal red gloss** | **RAL 3020 Traffic Red, ~#CC1611.** Fenced: NOT orange / orange-red / vermilion / coral / scarlet / tomato, NOT pink / magenta / maroon / burgundy / crimson / brick / rust. **Smooth high gloss 85–90 GU**, tight hard-edged specular ribbon on each tube crown, softer bounce highlight along the lower edge, subtle orange-peel allowed, **no mirrored surroundings**, not chrome/candy/metallic. | LCB, UCB, PC, UPC recolours |
| **KTM orange** | **KTM Racing Orange, ~RAL 2004, ~#F35B04**, slight red lean. Fenced: NOT yellow / amber / gold / tan / peach / coral, NOT red / scarlet / brown / rust. **Textured, ~15 GU**, not gloss. Orange shadows stay orange. Insides of bores and tube ends are orange, not black voids. | KTM protection combo, black→orange two-tone |
| **Neutral white** | Clean pure **neutral** white: NOT cream / ivory / beige / off-white / warm / blue-white / grey. Same textured coat. Weld beads turn white too. **Exposure ceiling ~80% brightness**, plus the plastic test (if any panel looks like smooth plastic, it's over-exposed). | White recolours |

**Placeholder colours in OM CAD:** orange (skid plate, KTM combo), yellow (crash bars, pannier
rack, protection-combo bars), grey (protection-combo plate), red + yellow (luggage combo
sub-assemblies). Every prompt says the placeholder is **not** the product colour.

## Hardware

- **If it's a threaded fastener, it's polished stainless. If it's structural metal, it's painted.**
  Only bolt heads, nuts, washers and exposed thread are stainless. Clamp collar bodies, saddles, spacers,
  standoffs, tabs, brackets and straps are always painted, "no matter how small or hardware-like it looks".
- **Stainless spec:** bright silver metallic, clean slightly reflective sheen, crisp specular highlight.
  NEVER black, dark, powder-coated or dull zinc.
  *Two older prompts (crash bars rendered, crash bars → white from reference) still say "zinc-plated
  silver". Every newer prompt says polished stainless.*
- **Size:** small, compact, sitting flush. Roughly **M8, ~13mm across the flats**. Test: if a bolt
  reads as a prominent feature, it's far too big.
- **How to identify hardware in the CAD:**
  - **Silver test** (the CAD shows fasteners in silver): render a fastener only where the CAD shows a
    bright silver shape. A hole is never an invitation for a bolt. "Ending with FEWER fasteners is a
    lesser error than adding even one that isn't there."
  - **Shape test** (the CAD is all one colour, e.g. KTM combo): anything shaped like a hex head, nut,
    washer or threaded shaft is hardware and is rendered stainless, even though the CAD shows it orange.
- **Never** add a fastener to balance, match, mirror or complete another. **Never** omit one the
  CAD shows. Count before, count after.
- **Clamp = two things at one spot:** a painted collar body plus stainless bolts. The coating never
  flows over its own hardware. Every clamp collar is a complete closed ring with two bolt ears.
- **No floating hardware:** every bolt passes through solid metal and ends in something.

## Welds: the hierarchy

Apply in this order. Each rule overrides the ones below it.

0. **Never weld a CAD artifact.** Tessellation, facet and body-split lines are software artifacts.
1. **Bolted joints are never welded.** Any fastener at a joint means no bead on it, around it or near it.
2. **A fold is never a weld** (sheet metal). Press-brake bends are clean radiused corners.
3. **Tube-to-tube, no fastener:** a continuous TIG bead wraps the junction.
4. **Flat meets round tube, no fastener:** a bead follows the contour.
5. **No flat-to-flat welds, and no mid-span welds** on straight or curved tube runs.
6. **Spacers and standoffs are loose sleeves.** They are never welded.

**Bead spec:** slightly raised, evenly spaced stack-of-dimes ripples ~3mm wide, crisp and controlled,
catching a soft highlight, never puffy or melted. Recolours: the coating goes over the welds, so
beads change colour but keep their raised relief.

## Backgrounds

| Background | When |
|---|---|
| **Plain solid pure white**, completely empty, with a soft grounded contact shadow as the only shadow | Default for every CAD → photo and every red/orange recolour (frozen) |
| **#6B6B6B neutral grey seamless**, smooth gradient lifted behind/above, floor is the darkest area | Single-part white hero (skid plate → white) |
| **#828282 mid-tone neutral grey** | White + black two-tone (protection combo → white) so both colours separate |
| **Dark charcoal matched to a reference image** | Crash bars → white from reference |

**Grounding, every time:** the part rests on the surface. Contact shadows are darkest and
tightest where metal meets the surface and fade outward. No detached or floating drop shadow. Clean
background shows through every hole and slot.

## Lighting styles

- **Catalogue (even):** bright, clean, high-key, large soft wraparound light from multiple
  directions, no dark pockets, and a specular ribbon on each tube crown. Used in the tail tidy, crash
  bars (rendered), reckless rack and protection combo prompts.
- **Sculptural premium (newer default):** high-key but *not flat*. Soft key from above-front with
  gentle fill, a crisp specular ribbon falling off to a richer shadowed side, and real tonal range.
  Used in the pannier rack, rear combo, luggage combo, crash bars (screenshot) and KTM combo prompts.
- **Cinematic (white on grey):** 45° key upper front-left, fill at ~⅓ strength, and a **rim/kicker
  from behind-above, the most important light**, so the white silhouette doesn't dissolve. The
  drama comes from deeper shadows, never hotter highlights.

## Camera

"Keep the exact same camera angle, viewpoint, orientation, rotation, perspective, and framing…
render-to-photograph; the viewpoint is locked to the input." Composition changes are **crop only**.
Strongest form (KTM combo): **the no-new-surfaces test**. If any face is visible that wasn't
visible in the CAD, the camera moved.

## OM plaque

Upload the Outback Motortek badge artwork as its own image. Canonical block (change only the
**PLACEMENT** sentence):

```text
OM PLAQUE (reproduce from the badge image, clean neutral colours only): add exactly ONE Outback Motortek plaque — a small rectangular emblem with rounded corners and a glossy domed-resin surface, showing the circular "OM" mark and the "OUTBACK MOTORTEK" wordmark on a deep black background with a crisp, bright WHITE / light-silver logo and text. NO blue tint, hue, glow, or cast anywhere. PLACEMENT: [see below]. One badge only, upright, reading correctly, about 40mm wide, not stretched, tilted, or repeated. The separate Outback Motortek badge image is ONLY the artwork source for the plaque — not the part, not the background, and it must not otherwise appear.
```

Placements already in use:

- **Crash bars / tail tidy:** flat against the straight lower horizontal cross-brace tube, centred,
  facing the camera, flush and conforming to the tube's gentle curve.
- **Reckless rack:** LEFT-HAND arm only (the piece on the left of the image), on a clearly visible
  straight tube section. Never the right arm, never a tab.
- **Protection combo:** a large, clearly visible flat panel face of the skid plate, near a lower
  area, lying flush. Never on a round tube.

## Recolour freeze block

Every recolour ends with the same freezes. Keep all six:
**hardware count, geometry, welds, camera, lighting, background**, plus "render quality: hold
it at the original level". Final checks are written as a **hunt** ("scan the image for anything
still black"), never a confirmation.

## Repeat offenders

These are the failures the prompts call out by name, and the lines that fixed them:

| Failure | Where | Fix line |
|---|---|---|
| Nuts come out M12 instead of M8 | Skid plate | Absolute size + "1/30th of the plate's length" + "if you notice it first, it's too big" |
| Hardware invented in holes / on the spacer | Skid plate, pannier, rear combo | Silver test + named zero-hardware zones |
| Clamp bolts painted with the collar | Black→orange, KTM combo | "A clamp is two things at one spot" |
| Top strap/bracket recoloured with the bars | UPC | Dedicated SWEEP 1 in the final check |
| White blown out into plastic | White recolours | ~80% ceiling + plastic test |
| Part floating | Grey backdrops | "The floor area is the darkest part of the backdrop" |
| Mirrored twin of a one-sided bracket | KTM combo | "Never mirror, duplicate or add a component" |
| Tessellation lines turned into weld rings | Crash bars screenshot | CAD-artifact block + weld RULE 0 |
