# Crash Bars / Engine Guards — CAD → Photo

Mandrel-bent tubular crash bars with bolted clamp-collar cross brace, textured black powder coat, on pure white. Two versions, depending on what you export from CAD, plus an optional OM plaque add-on.

**Model:** Nano Banana Pro on Higgsfield  
**Upload:** Image 1: the CAD image (yellow placeholder colour). Add the badge artwork as Image 2 only when using the plaque add-on.

### Before you paste

- **Which version?**
  - **Non-rendered:** use it when the upload is a *CAD viewport screenshot* showing tessellation/facet lines on the tubes. It tells the model those lines are software artifacts, not welds.
  - **Rendered:** use it when the upload is a clean CAD render.
- The **Rendered** version calls fasteners *zinc-plated silver*, while every other OM prompt says *polished stainless*. Change it to stainless if that's the current standard.
- The plaque goes on the lower horizontal cross-brace tube. Paste the add-on at the end of either version.

### What this prompt is guarding against

- Tessellation/body-split lines turned into weld rings → "CAD software artifacts — ignore them completely" + weld RULE 0
- Hardware invented in empty tab holes, or real clamp hardware deleted → "transfer from the CAD only, both directions" + count before and after
- Clamp collar bodies rendered as bare metal → "structural parts are always black"
- Cross brace deleted, floated or merged → explicit preserve instruction
- Phantom/doubled tubes where bars cross → overlap instruction

---

## Version A — Non-rendered CAD screenshot

**12,812 characters**

```text
Turn the uploaded CAD image into a photorealistic studio product photograph of the same motorcycle crash bars / engine guards. This is a re-render of the exact image provided, not a new shot.

REFERENCE IMAGES: the main CAD image is the part to photograph.

═══════════════════════════════════════════════════════════════════════════
CAD SOFTWARE ARTIFACTS — IGNORE THEM COMPLETELY (CRITICAL)
═══════════════════════════════════════════════════════════════════════════

The uploaded image is a CAD VIEWPORT SCREENSHOT, not a finished photorealistic render. It contains software display artifacts that are NOT real physical features of the product:

• Faint SEGMENT / TESSELLATION / FACET LINES running around and along the tubes, where the CAD software subdivides curved surfaces into flat polygons
• BODY SPLIT LINES where separate CAD bodies or components meet along a tube
• Mesh triangulation edges, isoparametric curves, and surface patch boundaries
• Slightly angular or polygonal-looking curves caused by low-resolution display tessellation

IGNORE ALL OF THESE. They are screen artifacts, not metal features. Do NOT interpret any of these lines as weld beads, weld rings, bend lines, seams, joints, panel gaps, ridges, creases, grooves, or surface detail of any kind.

THE REAL TUBES ARE PERFECTLY SMOOTH: every tube is one continuous, unbroken, seamless piece of mandrel-bent steel — flawlessly smooth along its entire length with no rings, bands, lines, segments, ridges, or interruptions anywhere on its surface. Curves and bends are perfectly smooth and round, never faceted, angular, or segmented. Render the tubes as the smooth continuous metal they actually are, and place weld beads ONLY where the WELDS section below explicitly permits them.

═══════════════════════════════════════════════════════════════════════════
RULE ZERO — HARDWARE: TRANSFER FROM THE CAD ONLY, BOTH DIRECTIONS
═══════════════════════════════════════════════════════════════════════════

Hardware is copied one-to-one from the CAD. Fasteners appear in the CAD as small, discrete, BRIGHT SILVER / CHROME / GREY-METALLIC components — compact hex bolt heads, nuts, and thin washers — clearly distinct from the yellow painted tubes and tabs.

NEVER INVENT: do not add any bolt, nut, washer, or fastener the CAD does not show. Apply this test to every fastener before rendering it:

• Does the CAD show a small BRIGHT SILVER/CHROME fastener at this exact spot? → YES: render it.
• Is this spot just a HOLE — dark, empty, recessed, or the same colour as the surrounding metal? → NO HARDWARE. Render a clean, empty, open hole. Nothing in it.

The plain holes in the flat mounting tabs and feet are EMPTY by design — the customer's own bolts go there at installation. A hole is NOT an invitation to add a bolt. Never add a fastener to "balance" or "match" another, or for symmetry or visual completeness.

NEVER OMIT: equally, do not delete, hide, or clean away any bolt, nut, washer, clamp, or collar assembly the CAD DOES show. Every fastener visible in the CAD must appear in the output, in the same position, quantity, and style. Count the fasteners in the CAD before rendering, then confirm the output has the same count in the same places — no more, no fewer.

HARDWARE FINISH — ALWAYS STAINLESS STEEL: every fastener is polished STAINLESS STEEL — bright silver metallic with a clean, slightly reflective sheen and a crisp specular highlight, clearly distinct against the black powder coat. NEVER black, NEVER dark, NEVER powder-coated, NEVER dull zinc.

HARDWARE SIZE AND SHAPE: reproduce each fastener at the exact modest scale shown in the CAD — small, neat hex bolt heads with thin flat washers and compact hex nuts, sitting tight and flush against their joint. Do NOT render fasteners oversized, chunky, bulbous, or blobby. Do NOT extend any bolt shaft or threaded rod out into open space. Hex heads are crisp six-sided shapes with clean flats and sharp corners.

STRUCTURAL PARTS ARE ALWAYS BLACK: every tube, mounting tab, bracket, gusset, foot, saddle, and CLAMP COLLAR BODY is textured black powder coat — no matter how small or hardware-like it looks. The clamp collar bodies (the metal saddle/strap pieces wrapping the tube) are structural steel and are BLACK, not silver, not zinc, not bare metal. Do NOT render any collar, saddle, bracket, tab, or foot in bare aluminium or raw metal. The ONLY stainless items in the entire image are threaded fasteners: bolt heads, nuts, and washers. If it is a threaded fastener it is stainless; if it is structural metal it is black.

BEFORE FINISHING, AUDIT every fastener in your output. Confirm each corresponds to a bright silver fastener at that exact location in the CAD, and that none from the CAD are missing.

═══════════════════════════════════════════════════════════════════════════

CAMERA — MOST IMPORTANT GEOMETRY RULE: keep the exact same camera angle, viewpoint, orientation, rotation, perspective, and framing as the uploaded CAD image. Reproduce that identical view. Do NOT rotate, tilt, re-angle, zoom, recompose, or move the camera. Only render changes — render-to-photograph; the viewpoint is locked to the input.

PRESERVE PROPORTIONS — TRUE SHAPE, NO SQUISH: keep the part's true real-world proportions and aspect ratio exactly as in the CAD. Do NOT scale non-uniformly, stretch, squash, elongate, widen, compress, or foreshorten in any direction. Present the whole assembly at a generous, consistent size filling most of the frame with even margins, scaled UNIFORMLY only (equal scale in every direction).

CRITICAL — EXACT GEOMETRY, ADD NOTHING: reproduce the CAD's exact structure — every tube, bend, curve, junction, mounting tab, bracket, gusset, foot, and hole in the same positions and count. Do NOT invent, add, duplicate, or reshape anything. Every fitting maps one-to-one to a fitting in the CAD.

Preserve the horizontal cross-brace tube and its connection points to the main bars exactly as the CAD shows — including the clamped/bolted collar assemblies at each end where it meets the main bars. Do NOT delete, simplify, merge, or float the cross brace; it stays fully connected exactly as modeled.

Pay special attention where tubes OVERLAP, CROSS, or PASS BEHIND one another — render ONLY the tubes present in the CAD, with no phantom, echoed, doubled, or extra tubing anywhere. The total count of tubes and their exact paths must match the CAD one-to-one.

GEOMETRY: preserve every tube, bend, curve, junction, mounting tab, bracket, gusset, foot, clamp collar, and hole exactly as shown, at the exact positions and proportions in the CAD. Keep tube diameters and bend radii identical. Add nothing, remove nothing, reshape nothing. Holes stay holes — reproducing a hole means rendering an empty opening, never filling it with a fastener.

MATERIAL — IGNORE THE CAD'S PLACEHOLDER COLOUR: the CAD uses yellow as a placeholder. In the real product EVERY structural component — all tubes, tabs, brackets, gussets, feet, saddles, and clamp collar bodies — is finished in ONE single uniform textured BLACK powder coat. There is no yellow, no two-tone, and no colour difference between any parts.

Mandrel-bent tubular steel with laser-cut steel tabs and feet. The coating has a fine, even, sandy micro-grain across every surface — low gloss, roughly 15 gloss units, scattering light into soft broad highlights rather than sharp mirror reflections. Deep, rich, saturated neutral black with real depth — never washed out, grey, dull, or flat. No blue or brown cast. The grain must be clearly readable so it reads as a genuine powder-coated part, not a smooth or lifeless 3D surface. HIGHLIGHTS: a bright, crisp specular ribbon rides the crown of each round tube to reveal its round cross-section.

═══ WELDS — STRICT HIERARCHY, IN THIS ORDER OF PRECEDENCE ═══

RULE 0 — NEVER WELD A CAD ARTIFACT: the segment, tessellation, facet, and body-split lines visible on the tubes in the CAD image are software artifacts, NOT weld locations. Do NOT place a weld bead, ring, band, or seam anywhere along a tube's length just because a line appears there in the CAD. Tube surfaces are smooth and unbroken between real junctions.

RULE 1 — BOLTED JOINTS ARE NEVER WELDED (overrides everything below): if a joint has ANY fastener at it — bolt, nut, screw, or washer — that joint is BOLTED and gets absolutely NO weld bead. Not on it, not around it, not near it. A bolt and a weld are mutually exclusive. The clamped cross-brace collar assemblies are BOLTED — render their stainless hardware and leave those joints completely clean with no weld texture whatsoever. If you see hardware at a joint, do not weld it.

RULE 2 — WELDED TUBE-TO-TUBE JUNCTIONS: where one tube is permanently welded directly to another tube with no fastener present, a continuous TIG bead wraps that junction fully — slightly raised, evenly spaced stack-of-dimes ripples about 3mm wide, catching a soft highlight along each ripple.

RULE 3 — WELDS WHERE FLAT MEETS ROUND TUBE, NO FASTENER: a bead appears where a flat mounting tab, bracket, gusset, or foot is permanently fixed directly onto a ROUND TUBE with no fastener present, following the contour where the flat piece meets the tube's curved surface.

RULE 4 — NO FLAT-TO-FLAT WELDS: never add a bead where one flat component meets another flat component — tab to bracket, bracket to bracket, collar to tab. A weld requires a ROUND TUBE on one side AND no hardware at the joint. If both sides are flat, there is no weld.

RULE 5 — NO MID-SPAN WELDS: absolutely no weld beads, rings, or bands along the smooth straight or curved runs of any tube. Between real junctions, tube surfaces are completely clean and unbroken.

Summary: weld beads exist ONLY at fastener-free tube-to-tube junctions and fastener-free flat-to-round-tube joints. No CAD artifact lines, no bolted joints, no flat-to-flat, no mid-span.

═══ BOLTED ASSEMBLIES — DISCRETE PIECES, NOT FUSED ═══

Where components are bolted together — the clamp collars around the cross-brace tube, tabs to brackets — they are SEPARATE physical pieces clamped by hardware, not one continuous fused mass. Render each with its own visible outline and edges, a crisp parting line where they meet, a visible step in material thickness where one sits against another, and a compact stainless fastener visibly clamping them. Do NOT blend, melt, fillet, or flow one component into another.

BACKGROUND: a plain, solid, pure white background — completely empty and featureless. No studio, softbox, light tent, diffusion panels, walls, corners, seams, floor line, props, motorcycle, or visible lighting gear. Nothing but flat, even, seamless white around the part. Clean white shows through every open loop and hole.

GROUNDING & CONTACT SHADOW: the part RESTS naturally on the white surface — its feet and lowest points make solid physical contact with the ground, sitting firmly and stably. It is NOT floating, hovering, or suspended in mid-air. At EVERY point where a foot or tube touches down, render a soft, realistic contact shadow anchored right at that contact point — darkest and tightest exactly where the metal meets the surface, fading softly outward. Those grounded contact shadows are the only shadows in the image. Do NOT render a single detached, offset, or floating drop shadow.

COMPOSITION — CENTERED: center the entire assembly horizontally and vertically within the frame, with even, balanced white space on all four sides. Do NOT push the subject to one side, corner, or edge. This is a framing/crop adjustment only — it does NOT change the camera angle, viewpoint, or perspective, which stay locked to the CAD.

LIGHTING: relight the part with rich, sculptural, premium studio lighting so every tube reads as strongly three-dimensional and round — a bright, crisp specular highlight ribbon along each tube crown falling off smoothly to a deeper, richer shadowed side, giving full roundness and form. This must NOT be flat, uniform, grey, or washed out. Keep a clean, bright, high-key feel with a soft key from above-front plus gentle fill, so recessed areas, inner-facing tubes, and rear tubes stay readable with no muddy black holes — but allow real tonal range and genuine depth in the shadows rather than lifting everything to a flat grey. Punchy, dimensional, high-end: deep rich blacks, clean bright highlights, strong sense of form on every tube.

RENDER QUALITY: photoreal, physically accurate materials, tack sharp, rich tonal contrast with deep true blacks and clean bright highlights, neutral true-to-life colour, subtle film grain, faint atmospheric depth, crushed blacks that retain shadow detail. Premium, punchy, and indistinguishable from a real high-end product photograph. Every tube surface is flawlessly smooth between real welded junctions.
```

## Version B — Rendered CAD

**5,446 characters**

```text
Turn the uploaded CAD render into a photorealistic studio product photograph of the same motorcycle crash bars / engine guards. This is a re-render of the exact image provided, not a new shot.

REFERENCE IMAGES: the main CAD render is the part to photograph.

CAMERA — MOST IMPORTANT RULE: keep the exact same camera angle, viewpoint, orientation, rotation, perspective, and framing as the uploaded image. Whatever angle the part is shown at — top-down, bird's-eye, side, front, three-quarter, or any other — reproduce that identical view. Do NOT rotate, tilt, re-angle, re-orient, zoom, recompose, or move the camera. The part must sit in the same position and at the same angle as the upload. The only thing that changes is render-to-photograph; the viewpoint is locked to the input.

GEOMETRY: preserve every tube, bend, curve, junction, mounting tab, bracket, foot, hole, and the overall proportions exactly as shown. Add nothing, remove nothing, reshape nothing. Keep the tube diameters and bend radii identical to the upload. Preserve the horizontal cross-brace tube and its connection points to the main bars exactly as the CAD shows — including the clamped/bolted collar assemblies at each end where it meets the main bars. Do NOT delete, simplify, merge, or float the cross brace; it stays fully connected exactly as modeled.

HARDWARE — TRANSFER FROM THE CAD ONLY, NEVER GENERATE: hardware is copied one-to-one from the CAD, in both directions. Do NOT invent or add any bolt, nut, washer, or fastener the CAD does not show — AND do NOT delete, omit, hide, or clean away any bolt, nut, washer, clamp, or collar assembly the CAD DOES show. Every fastener visible in the CAD must appear in the output, in the same position, the same quantity, and the same style; every location the CAD leaves bare must stay bare.

Specifically: where the CAD shows clamp/collar assemblies joining the cross-brace tube to the main bars, reproduce those exact assemblies in those exact positions — but split the finish correctly. The CLAMP COLLAR BODIES (the metal saddle/strap pieces wrapping the tube) are structural parts of the product and are finished in the SAME textured black powder coat as the tubes — NOT silver, NOT zinc, NOT bare metal. ONLY the fasteners themselves — the bolt heads, nuts, and washers — are bright zinc-plated silver. Black collar bodies, silver bolts.

Count the fasteners in the CAD before rendering, then confirm the output has the same count in the same places — no more, no fewer.

MATERIAL: mandrel-bent tubular steel, TIG-welded, with laser-cut steel mounting tabs and feet, finished in a textured black powder coat. The coating has a fine, even, sandy micro-grain across the whole surface — low gloss, roughly 15 gloss units, scattering light into soft broad highlights rather than sharp mirror reflections. Deep neutral black, no blue or brown cast. The grain must be clearly readable so it reads as a real powder-coated part, not a smooth 3D surface. Zinc-plated FASTENERS ONLY — bolt heads, nuts, and washers — keep their bright metallic silver finish. Every other component, including clamp collars, saddles, brackets, tabs, and feet, is powder coated black like the tubes. If a part is structural metal rather than a threaded fastener, it is black.

WELDS: a continuous TIG weld bead wraps every joint where one tube meets another tube, and every joint where a flat mounting tab, bracket, or foot is welded onto a tube — slightly raised, evenly spaced stack-of-dimes ripples about 3mm wide, fully encircling each tubular junction exactly as a real welder laid it, catching a soft highlight along each ripple. Do NOT add weld beads mid-span along the smooth straight or curved runs of tube — welds appear ONLY at actual tube-to-tube junctions and at tab/bracket/foot connections. The clamped cross-brace connections are BOLTED, not welded — render their hardware and leave those joints clean with no weld bead.

BACKGROUND: a plain, solid, pure white background — completely empty and featureless. No studio, no softbox, no light tent, no diffusion panels, no walls, no corners, no seams, no floor line, no props, no visible lighting equipment of any kind. Nothing but flat, even, seamless white around the part. A soft, low-contrast, light-grey contact shadow sits directly beneath the part where it meets the surface, tight at contact points and fading outward. That shadow is the only thing on the white besides the part.

LIGHTING: fully relight the part cleanly and professionally — ignore and correct any poor, uneven, dark, or underexposed lighting in the source render. Bright, clean, high-key commercial product lighting that evenly illuminates the ENTIRE part, every tube, tab, and surface, including recessed, inner-facing, and rear tubes. No dark patches, no muddy shadows, no underexposed pockets anywhere — push soft, generous fill light around and behind the tubes so no section falls into gloom. Use large, soft, wraparound illumination from multiple directions with gentle gradation, and let a clean specular highlight ribbon run along the top crown of each tube to reveal its round cross-section and define the form. Premium, evenly-lit catalogue look.

RENDER QUALITY: photoreal, physically accurate materials, tack sharp, neutral true-to-life colour, subtle film grain, faint atmospheric depth, gently crushed blacks with retained shadow detail. Indistinguishable from a real product photograph.
```

## Add-on — OM plaque

Paste at the end of Version A or B and upload the badge artwork as Image 2.

**1,042 characters**

```text
The separate Outback Motortek badge image is ONLY the artwork source for the plaque described below — it is not the part, not the background, and must not otherwise appear in the scene.

OM PLAQUE (reproduce from the provided badge image, but render it in clean neutral colours only): add exactly ONE Outback Motortek plaque — a small rectangular emblem with softly rounded corners and a glossy domed-resin surface, showing the circular "OM" logo mark and the "OUTBACK MOTORTEK" wordmark. Render it with a deep black background and a crisp, bright WHITE / light-silver logo and wordmark. NO blue tint, no blue hue, no blue glow, no blue colour cast anywhere on the badge — logo and text are clean neutral white/silver only, catching a soft neutral highlight across the domed top. Mount it flat against the straight lower horizontal cross-brace tube, centered and facing the camera, flush and conforming to the tube's gentle curve. One badge only, upright and reading correctly, about 40mm wide — not stretched, distorted, tilted, or repeated.
```
