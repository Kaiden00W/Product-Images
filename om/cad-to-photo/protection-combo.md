# Protection Combo (Crash Bars + Skid Plate) — CAD → Photo

Exploded view: tubular crash bars and a separate folded skid plate, spaced apart, both textured black powder coat, on pure white. Two versions.

**Model:** Nano Banana Pro on Higgsfield  
**Upload:** Image 1: the CAD render (yellow bars, grey plate placeholder). V1 also needs Image 2: the Outback Motortek badge artwork.

### Before you paste

- **V2 (newer)** uses the silver test for hardware and doesn't include the plaque.
- **V1** hard-codes that the skid plate's main body has **zero hardware**, with the only exception being countersunk bolts on the rear linkage guard flap. It also adds the OM plaque on a flat skid-plate panel. Check that rule against this CAD.
- Both keep the two pieces **apart** at the CAD's exact spacing. Neither version joins them.

### What this prompt is guarding against

- The model bridges the gap between the bars and the plate with an invented bracket → "two separate components… do NOT bring them together"
- Bolts added to skid-plate vent/panel holes → silver test (V2) / "skid plate is completely bolt-free" (V1)
- Brackets rendered as bare aluminium → "structural metal is black"

---

## V2 — Current

**8,153 characters**

```text
Turn the uploaded CAD render into a photorealistic studio product photograph of the same motorcycle crash bar + skid plate combo (tubular engine guards combined with a folded bash plate). This is a re-render of the exact image provided, not a new shot.

REFERENCE IMAGES: the main CAD render is the part to photograph.

═══ RULE ZERO — THE SILVER TEST FOR HARDWARE (READ FIRST, HIGHEST

PRIORITY) ═══

Hardware is identified by COLOUR in the CAD, not by the presence of holes.

In the CAD, real fasteners are rendered as small, discrete, BRIGHT CHROME/SILVER components — visible hex bolt heads, nuts, and washers — obviously separate little parts sitting proud of the surface, in a metallic silver clearly different from the painted tubes and panels.

Apply this test to every single fastener before you render it:

• Does the CAD show a small BRIGHT SILVER/CHROME fastener shape at this exact spot? → YES: render it.
• Is this spot just a HOLE — dark, empty, recessed, or the same colour as the surrounding panel/tube? → NO HARDWARE. Render it as a clean, empty, open hole. Nothing in it. Ever.

MOST HOLES IN THIS PRODUCT ARE EMPTY. Bare mounting holes, tab holes, plate holes, and vent slots are UNFILLED by design — they are where the customer's own bolts go during installation, so they ship empty. A hole is NOT an invitation to add a bolt.

Explicitly forbidden: adding a bolt to a plain tab hole. Adding bolts to the skid plate's flat panels or front flap holes. Adding a second bolt to "balance" or "match" a single one. Adding hardware for visual completeness, symmetry, or realism. If you feel an urge to add a fastener that you cannot point to as a silver shape in the CAD — do not add it.

Before finishing, audit every fastener in your output. For each one, confirm you can point to a bright silver fastener at that exact location in the CAD. Delete any you cannot. Ending with FEWER fasteners than the CAD is a lesser error than adding even one that isn't there.

══════════════════════════════════════════════════════════════════

CAMERA — LOCKED: keep the exact same camera angle, viewpoint, orientation, rotation, perspective, and framing as the uploaded CAD render. Reproduce that identical view. Do NOT rotate, tilt, re-angle, zoom, recompose, or move the camera. Only render changes — render-to-photograph; the viewpoint is locked to the input.

PRESERVE PROPORTIONS — TRUE SHAPE, NO SQUISH: keep the assembly's true real-world proportions and aspect ratio exactly as in the CAD. Do NOT scale non-uniformly, stretch, squash, elongate, widen, compress, or foreshorten in any direction. Present the whole combo at a generous, consistent size filling most of the frame with even margins, scaled UNIFORMLY only. It looks exactly as proportioned as in the CAD — only larger or smaller as a whole, never distorted.

CRITICAL — EXACT GEOMETRY, TWO SEPARATE COMPONENTS: this is an EXPLODED VIEW showing two separate, physically distinct components — round tubular crash bars as one piece, and a folded sheet-metal skid plate as a separate piece — deliberately spaced apart to display both clearly. They are NOT touching, NOT connected, NOT joined. Keep them as two distinct separate pieces at the exact same relative positions, spacing, gap distance, and orientation as the CAD. Do NOT bring them together, connect them, invent any bracket/tab/tube/weld bridging the gap, or reshape, merge, or reposition either piece. Every feature maps one-to-one to a feature in the CAD, same place and count. Where crash-bar tubes overlap, cross, or pass behind one another, render ONLY the tubes present in the CAD — no phantom, echoed, or extra tubing anywhere.

GEOMETRY: preserve every tube, bend, curve, junction, folded panel, bend line, cut-out, vent slot, mounting hole, bracket, tab, and foot exactly as shown, at the exact positions and proportions in the CAD. Keep tube diameters, bend radii, and panel folds identical. Add nothing, remove nothing, reshape nothing. Holes stay holes — reproducing a hole means rendering an empty opening, never filling it with a fastener (see RULE ZERO).

COMPOSITION — CENTERED: center the entire subject (both pieces together, as one composition) horizontally and vertically in the frame, with even, balanced white space on all four sides. Do NOT push the subject to one side, corner, or edge. This is a framing/crop adjustment only — it does NOT change the camera angle, viewpoint, or perspective, which stay locked to the CAD.

MATERIAL: mandrel-bent tubular steel crash bars and a laser-cut, press-brake-folded aluminium skid/bash plate, BOTH finished in the same uniform textured black powder coat — fine, even, sandy micro-grain across every surface, low gloss around 15 gloss units, soft broad highlights rather than sharp mirror reflections. Deep neutral black, no blue or brown cast. The grain must read as real powder coat, not a smooth 3D surface. Ignore the CAD's placeholder colours (yellow bars, grey plate) — both pieces are black in the real product. HIGHLIGHTS: a clean specular ribbon rides the crown of each round tube; broad soft highlights sweep across the flat skid-plate panels with a crisp bright line catching each folded edge.

HARDWARE FINISH — ALWAYS STAINLESS STEEL: every fastener that passes RULE ZERO — bolt heads, nuts, washers, countersunk flat-heads — is polished STAINLESS STEEL: bright silver metallic with a clean, slightly reflective sheen and a crisp specular highlight, clearly distinct against the black powder coat. Never black, never dark, never powder-coated. Fasteners are the ONLY stainless components. Every structural part — tubes, panels, brackets, tabs, feet, and clamp collar bodies — stays textured black powder coat. If it is a threaded fastener it is stainless; if it is structural metal it is black. Do NOT render any bracket, strap, plate, collar body, tab, or mounting piece in bare aluminium, raw metal, or stainless — no matter how small or hardware-like it appears. Those are all powder-coated black. The ONLY stainless items in the entire image are threaded fasteners: bolt heads, nuts, and washers. Everything else that is metal is black.

WELDS: on the tubular crash bars, a continuous TIG weld bead wraps every tube-to-tube junction and every joint where a tab, bracket, or tube-end meets another tube. On the folded skid plate, a hand-laid TIG weld bead runs each seam where two folded panels meet and where the plate's brackets/tabs are welded on. All beads slightly raised, evenly spaced stack-of-dimes ripples about 3mm wide, catching a soft highlight along each ripple. NO weld beads mid-span on smooth tube runs or across the middle of a flat panel — only at real tube junctions, folded seams, and bracket/tab connections. Any joint that RULE ZERO renders as bolted is a BOLTED connection only — leave it clean with NO weld bead on, around, or near it.

BACKGROUND: a plain, solid, pure white background — completely empty and featureless. No studio, softbox, light tent, diffusion panels, walls, corners, seams, floor line, props, motorcycle, or visible lighting gear. Nothing but flat, even, seamless white. Clean white shows through every vent slot, cut-out, and empty mounting hole. A soft, low-contrast, light-grey contact shadow sits directly beneath the part, tight at contact points and fading outward — the only thing on the white besides the part.

LIGHTING: fully relight the assembly cleanly — correct any poor, uneven, or dark lighting from the source. Bright, clean, high-key product lighting that evenly illuminates the ENTIRE assembly — every tube, panel, tab, and surface, including recessed, inner-facing, and rear areas and the underside of the bars. No dark patches, no muddy shadows, no underexposed pockets — push soft fill light into every recess. Large, soft, wraparound illumination from multiple directions with gentle gradation. Premium, evenly-lit catalogue look.

RENDER QUALITY: photoreal, physically accurate materials, tack sharp, neutral true-to-life colour, subtle film grain, faint atmospheric depth, gently crushed blacks with retained shadow detail. Indistinguishable from a real product photograph.
```

## V1 — With OM plaque on the skid plate

**8,595 characters**

```text
Turn the uploaded CAD render into a photorealistic studio product photograph of the same motorcycle crash bar + skid plate combo (tubular engine guards combined with a folded bash plate). This is a re-render of the exact image provided, not a new shot.

REFERENCE IMAGES: the main CAD render is the part to photograph.

CAMERA — MOST IMPORTANT RULE: keep the exact same camera angle, viewpoint, orientation, rotation, perspective, and framing as the uploaded CAD render. Reproduce that identical view. Do NOT rotate, tilt, re-angle, zoom, recompose, or move the camera. Only render changes — render-to-photograph; the viewpoint is locked to the input.

PRESERVE PROPORTIONS — TRUE SHAPE, NO SQUISH: keep the assembly's true real-world proportions and aspect ratio exactly as in the CAD. Do NOT scale non-uniformly, stretch, squash, elongate, widen, compress, or foreshorten in any direction. Present the whole combo at a generous, consistent size filling most of the frame with even margins, scaled UNIFORMLY only. It looks exactly as proportioned as in the CAD — only larger or smaller as a whole, never distorted.

CRITICAL — EXACT GEOMETRY, TWO SEPARATE COMPONENTS, ADD NOTHING: this is an EXPLODED VIEW showing two separate, physically distinct components of a crash bar + skid plate combo — round tubular crash bars as one piece, and a folded sheet-metal skid plate as a separate piece — deliberately spaced apart in the air to display both clearly. They are NOT touching, NOT connected, and NOT joined in this image. Keep them as two distinct separate pieces, at the exact same relative positions, spacing, gap distance, and orientation to each other as shown in the CAD. Do NOT bring them together, do NOT connect them, do NOT invent any bracket, tab, tube, or weld bridging the gap between them, and do NOT reshape, merge, or reposition either piece. Every feature in the output maps one-to-one to a feature in the CAD, in the same place and count. Pay special attention where the crash-bar tubes overlap, cross, or pass behind one another within that piece — render ONLY the tubes present in the CAD, with no phantom, echoed, or extra tubing anywhere.

GEOMETRY: preserve every tube, bend, curve, junction, folded panel, bend line, cut-out, vent slot, mounting hole, bracket, tab, foot, bolt, and nut exactly as shown, at the exact positions and proportions in the CAD. Keep tube diameters, bend radii, and panel folds identical. Add nothing, remove nothing, reshape nothing.

COMPOSITION — CENTERED: center the entire subject (both pieces, together, treating the exploded pair as one composition) horizontally and vertically within the frame, with even, balanced white space on all four sides — left, right, top, and bottom margins should be visually similar. Do NOT push the subject to one side, corner, or edge of the frame. This is a framing/crop adjustment only — it does NOT change the camera angle, viewpoint, or perspective, which stay exactly locked to the CAD.

MATERIAL: a combined assembly of mandrel-bent tubular steel crash bars and a laser-cut, press-brake-folded aluminium skid/bash plate, joined by welded steel brackets and tabs, finished in a single uniform textured black powder coat — fine, even, sandy micro-grain across every surface, low gloss around 15 gloss units, soft broad highlights rather than sharp mirror reflections. Deep neutral black, no blue or brown cast. The grain must read as real powder coat, not a smooth 3D surface. HIGHLIGHTS: a clean specular ribbon rides the crown of each round tube to reveal its cross-section; broad soft highlights sweep across the flat skid-plate panels with a crisp bright line catching each folded edge. All threaded fasteners are excluded from the powder coat — they are polished stainless steel, bright silver, never black.

HARDWARE — SKID PLATE IS COMPLETELY BOLT-FREE, NO EXCEPTIONS EXCEPT ONE:

The main body of the skid plate has ZERO hardware of any kind. Every hole, vent slot, and mounting hole on the skid plate's main panels — including all round holes, all vent slots, and every surface of the plate — is a plain, clean, empty, unthreaded opening. Do NOT render any bolt, screw, washer, nut, rivet, or fastener anywhere on the skid plate's main body. None. Zero. If you are unsure whether a hole should have a fastener, it does NOT — leave it empty.

THE ONE EXCEPTION: only at the rear linkage guard plate — the small separate flap/tab section at the rear of the skid plate — render the fastener(s) exactly as the CAD shows, as flush countersunk flat-head bolts (head fully recessed, level with the surface, tapered to the countersink, visible hex/Allen drive recess). This is the ONLY location on the entire skid plate where any hardware may appear.

CRASH BAR NUT/BOLT ASSEMBLIES: at the tube-to-bracket junctions where the CAD shows a small hex nut and washer, reproduce that exact hardware in that exact position and count — nothing added or removed. This is separate from the skid plate and unaffected by the no-hardware rule above.

HARDWARE FINISH — ALWAYS STAINLESS STEEL: every fastener rendered anywhere in this image — bolt heads, nuts, washers, countersunk flat-heads, on both the crash bars and the skid plate — is polished STAINLESS STEEL: bright silver metallic with a clean, slightly reflective sheen and a crisp specular highlight, clearly distinct against the black powder coat. Never black, never dark, never powder-coated, never zinc-dull. Fasteners are the ONLY stainless components — every structural part (tubes, panels, brackets, tabs, feet, clamp collar bodies) stays textured black powder coat. If a part is a threaded fastener it is stainless steel; if it is structural metal it is black.

WELDS: on the tubular crash bars, a continuous TIG weld bead wraps every tube-to-tube junction and every joint where a tab, bracket, or tube-end meets another tube. On the folded skid plate, a hand-laid TIG weld bead runs each seam where two folded panels meet and where the plate's brackets/tabs are welded on. All beads slightly raised, evenly spaced stack-of-dimes ripples about 3mm wide, catching a soft highlight along each ripple. NO weld beads mid-span on smooth tube runs or across the middle of a flat panel — only at real tube junctions, folded seams, and bracket/tab connections.

The bolted flat mounting tab at the rear of the skid plate (where visible bolts pass through) is a BOLTED connection only — render the bolts there and leave that joint completely clean with NO weld bead on, around, or near it.

BACKGROUND: a plain, solid, pure white background — completely empty and featureless. No studio, softbox, light tent, diffusion panels, walls, corners, seams, floor line, props, motorcycle, or visible lighting gear. Nothing but flat, even, seamless white. Clean white shows through every vent slot and cut-out in the skid plate. A soft, low-contrast, light-grey contact shadow sits directly beneath the part, tight at contact points and fading outward — the only thing on the white besides the part.

LIGHTING: fully relight the assembly cleanly — correct any poor, uneven, or dark lighting from the source. Bright, clean, high-key product lighting that evenly illuminates the ENTIRE assembly — every tube, panel, tab, and surface, including recessed, inner-facing, and rear areas and the underside of the bars. No dark patches, no muddy shadows, no underexposed pockets — push soft fill light into every recess. Large, soft, wraparound illumination from multiple directions with gentle gradation. Premium, evenly-lit catalogue look.

RENDER QUALITY: photoreal, physically accurate materials, tack sharp, neutral true-to-life colour, subtle film grain, faint atmospheric depth, gently crushed blacks with retained shadow detail. Indistinguishable from a real product photograph.

OM PLAQUE (reproduce from the badge image, clean neutral colours only): add exactly ONE Outback Motortek plaque — a small rectangular emblem with rounded corners and a glossy domed-resin surface, showing the circular "OM" mark and the "OUTBACK MOTORTEK" wordmark on a deep black background with a crisp, bright WHITE / light-silver logo and text. NO blue tint, hue, glow, or cast anywhere. Mount it flat on a large, clearly visible flat panel face of the skid plate, near a lower area, lying perfectly flush, upright and reading correctly to the camera, about 40mm wide — not stretched, tilted, repeated, or placed on a round tube. The separate Outback Motortek badge image is ONLY the artwork source for the plaque — not the part, not the background, and it must not otherwise appear.
```
