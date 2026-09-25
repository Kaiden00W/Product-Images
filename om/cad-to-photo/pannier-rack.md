# Pannier Rack — CAD → Photo

Side-case luggage carrier: two open rectangular tubular side frames with cross tubes and clamp collars, textured black powder coat, on pure white. Two versions.

**Model:** Nano Banana Pro on Higgsfield  
**Upload:** Image 1: the CAD render (yellow placeholder colour).

### Before you paste

- **Which version?**
  - **Version A (with mounting plates):** for a rack that has flat pannier mounting plates with a grid of holes and spacers/standoffs.
  - **Version B (standard, tube only):** for a rack that is almost entirely round tube plus a few small tabs and one strap. It explicitly forbids inventing any flat plate or hole grid.
- Using A on a tube-only rack invites the model to add plates. Using B on a plated rack tells it to delete them.

### What this prompt is guarding against

- Bolts added to every hole in the plate grid → the silver test + "most openings on this product are empty"
- Side frames rendered small/squashed → "FULL, OPEN, correctly-proportioned rectangles"
- Rack turned into crash bars / a basket / a cage → explicit structure description
- Spacers welded → "spacers and standoffs are loose sleeves, never welded"
- Invented feet, nubs and protruding studs (Version B) → explicit forbidden list

---

## Version A — With pannier mounting plates

**12,328 characters**

```text
Turn the uploaded CAD render into a photorealistic studio product photograph of the same motorcycle pannier rack / side-case luggage carrier. This is a re-render of the exact image provided, not a new shot.

REFERENCE IMAGES: the main CAD render is the part to photograph.

═══════════════════════════════════════════════════════════════════════════
RULE ZERO — HARDWARE: THE SILVER TEST (READ FIRST, HIGHEST PRIORITY)
═══════════════════════════════════════════════════════════════════════════

Hardware is identified by COLOUR in the CAD, not by the presence of holes. Real fasteners render in the CAD as small, discrete, BRIGHT SILVER / CHROME / GREY-METALLIC components — visible hex bolt heads, nuts, and washers — clearly distinct from the painted yellow tubes and plates.

Apply this test to EVERY fastener before rendering it:

• Does the CAD show a small BRIGHT SILVER/CHROME fastener at this exact spot? → YES: render it.
• Is this spot just a HOLE or SLOT — dark, empty, recessed, or the same colour as the surrounding metal? → NO HARDWARE. Render a clean, empty, open hole. Nothing in it. Ever.

MOST OPENINGS ON THIS PRODUCT ARE EMPTY. The grid of round holes across the flat pannier mounting plates, the elongated slots in the rectangular side frames, the eyelet holes in the mounting tabs, and every plain hole ship unfilled by design — the customer's own hardware goes there at installation. A hole is NOT an invitation to add a bolt.

EXPLICITLY FORBIDDEN: adding a bolt to any of the plate's grid holes, to a frame slot, to a plain tab or eyelet. Adding a fastener to "balance" or "match" another. Adding hardware for symmetry, visual completeness, or realism. If you feel an urge to add a fastener you cannot point to as a silver shape in the CAD — do not add it.

HARDWARE FINISH — ALWAYS STAINLESS STEEL: every fastener is polished STAINLESS STEEL — bright silver metallic with a clean, slightly reflective sheen and a crisp specular highlight, clearly distinct against the black powder coat. NEVER black, NEVER dark, NEVER powder-coated, NEVER dull zinc.

HARDWARE TYPE — MATCH THE HEAD STYLE AND SIZE EXACTLY: reproduce each fastener's exact head style, size, and proportion as modeled in the CAD — compact hex bolt heads with thin flat washers and hex nuts, sized realistically to the part. Do NOT render fasteners oversized, chunky, bulbous, or blobby. Do NOT substitute a domed button head for a hex head or vice versa. Where the CAD shows a hex head, render a crisp six-sided hex head with clean flats and sharp corners.

HARDWARE ORIENTATION: present each visible bolt with its clean hex head facing OUTWARD — toward the viewer and away from the centre of the rack. Never show the threaded shaft tip or the back/nut side facing outward. Orient existing fasteners head-out; do NOT add or remove any.

STRUCTURAL PARTS ARE ALWAYS BLACK: every tube, flat pannier mounting plate, rectangular side frame, mounting tab, hook, pin/stud, foot, bracket, gusset, spacer, standoff, and clamp collar body is textured black powder coat — no matter how small or hardware-like it looks. Do NOT render any bracket, collar, spacer, standoff, or plate in bare aluminium, raw metal, or stainless. The ONLY stainless items in the entire image are threaded fasteners: bolt heads, nuts, and washers. If it is a threaded fastener it is stainless; if it is structural metal it is black.

BEFORE FINISHING, AUDIT every fastener in your output. Confirm you can point to a bright silver fastener at that exact location in the CAD. Delete any you cannot. Ending with FEWER fasteners is a lesser error than adding even one that isn't there.

═══════════════════════════════════════════════════════════════════════════

CAMERA — MOST IMPORTANT GEOMETRY RULE: keep the exact same camera angle, viewpoint, orientation, rotation, perspective, and framing as the uploaded CAD render. Reproduce that identical view. Do NOT rotate, tilt, re-angle, zoom, recompose, or move the camera. Only render changes — render-to-photograph; the viewpoint is locked to the input.

PRESERVE PROPORTIONS — TRUE SHAPE, NO SQUISH: keep the part's true real-world proportions and aspect ratio exactly as in the CAD. Do NOT scale non-uniformly, stretch, squash, elongate, widen, compress, or foreshorten in any direction. The rectangular side frames must render as FULL, OPEN, correctly-proportioned rectangles — never small, shrunken, squished, flattened, or narrowed; they must match the true rectangle shape and size relationship of the CAD. Present the whole rack at a generous, consistent size filling most of the frame with comfortable, even margins on all sides, scaled UNIFORMLY only (equal scale in every direction).

CRITICAL — EXACT GEOMETRY, ADD NOTHING: this is a PANNIER RACK — a pair of large, open, rectangular tubular side frames with flat pannier mounting plates, joined by connecting cross tubes, with mounting pins/studs, hooks, tabs, brackets, and clamp collars. Keep that exact wide, open, rectangular structure. Do NOT compact or densify it, do NOT turn it into crash bars, a box, a basket, or a cage. Do NOT invent, add, or duplicate any extra tube, tab, eyelet, bracket, pin, plate, or fastener. Every fitting maps one-to-one to a fitting in the CAD, in the same place and count.

Pay special attention where tubes OVERLAP, CROSS, or PASS BEHIND one another — especially around the connecting cross tubes and where the frames meet the mounting plates. Render ONLY the tubes present in the CAD, with no phantom, echoed, doubled, or extra tubing anywhere. The total count of tubes and their exact paths must match the CAD one-to-one.

GEOMETRY: preserve every tube, bend, junction, rectangular loop, flat mounting plate and its exact outline, every hole in the plate grid, every frame slot, pannier pin/stud, hook, tab, bracket, foot, spacer, and clamp collar exactly as shown, at the exact positions and proportions in the CAD. Keep tube diameters and bend radii identical. Add nothing, remove nothing, reshape nothing. Holes stay holes — reproducing a hole means rendering an empty opening, never filling it with a fastener.

MATERIAL — IGNORE THE CAD'S PLACEHOLDER COLOUR: the CAD uses yellow as a placeholder. In the real product EVERY structural component — all tubes, side frames, mounting plates, tabs, hooks, pins, brackets, spacers, and clamp collar bodies — is finished in ONE single uniform textured BLACK powder coat. There is no yellow, no two-tone, and no colour difference between any parts.

The coating has a fine, even, sandy micro-grain across every surface — low gloss, roughly 15 gloss units, scattering light into soft broad highlights rather than sharp mirror reflections. Deep, rich, saturated neutral black with real depth — never washed out, grey, dull, or flat. No blue or brown cast. The grain must be clearly readable up close so it reads as a genuine powder-coated part, not a smooth or lifeless 3D surface. HIGHLIGHTS: a bright, crisp specular ribbon rides the crown of each round tube to reveal its round cross-section; broad soft highlights sweep across the flat mounting plates with a crisp bright line catching each edge.

═══ WELDS — STRICT HIERARCHY, IN THIS ORDER OF PRECEDENCE ═══

RULE 1 — BOLTED JOINTS ARE NEVER WELDED (overrides everything below): if a joint has ANY fastener at it — bolt, nut, screw, or washer — that joint is BOLTED and gets absolutely NO weld bead. Not on it, not around it, not near it. A bolt and a weld are mutually exclusive. This applies even when a round tube is involved. The clamp collars and every bolted tube-to-tube connection are BOLTED assemblies — render their stainless hardware and leave those joints completely clean with no weld texture whatsoever. If you see hardware at a joint, do not weld it.

RULE 2 — SPACERS AND STANDOFFS ARE LOOSE SLEEVES, NEVER WELDED: the small cylindrical spacers/standoffs between the mounting plates and the frames are separate slip-on components held by a bolt passing through them. Render each as a distinct piece with its own crisp end edges and a visible parting line where each end butts against the adjoining face, with smooth uninterrupted powder-coated metal at both ends. Absolutely NO weld bead on them, around them, at their bases, or at either end.

RULE 3 — WELDS APPEAR ONLY WHERE FLAT MEETS ROUND TUBE, WITH NO FASTENER: a TIG weld bead appears only where a flat component is permanently fixed directly onto a ROUND TUBE and no fastener is present — a mounting tab, hook, pin, foot, or gusset welded onto the tube itself. Slightly raised, evenly spaced stack-of-dimes ripples about 3mm wide, following the joint and catching a soft highlight.

RULE 4 — WELDED TUBE-TO-TUBE JUNCTIONS: where one tube is permanently welded directly to another tube with no fastener present, a continuous bead wraps that junction fully.

RULE 5 — NO FLAT-TO-FLAT WELDS: never add a bead where one flat component meets another flat component — plate to bracket, bracket to bracket, tab to tab, collar to plate. A weld requires a ROUND TUBE on one side of the joint AND no hardware present. If both sides are flat plate, there is no weld.

RULE 6 — NO MID-SPAN WELDS: no weld beads along the smooth straight or curved runs of any tube.

Summary: weld beads exist ONLY at fastener-free tube junctions and fastener-free flat-to-round-tube joints. No bolted joints, no spacers, no flat-to-flat, no mid-span.

═══ BOLTED ASSEMBLIES — DISCRETE PIECES, NOT FUSED ═══

Where two components are bolted together — clamp collars around tubes, mounting plates to frames, cross tubes to side frames — they are SEPARATE physical pieces clamped by hardware, not one continuous fused mass. Render each with its own visible outline and edges, a crisp parting line where they meet, a visible step in material thickness where one sits against the other, and a stainless fastener visibly clamping them. Do NOT blend, melt, fillet, or flow one component smoothly into another.

BACKGROUND: a plain, solid, pure white background — completely empty and featureless. No studio, softbox, light tent, diffusion panels, walls, corners, seams, floor line, props, motorcycle, or visible lighting gear. Nothing but flat, even, seamless white. Clean white shows through every open rectangular frame, plate hole, and slot.

GROUNDING & CONTACT SHADOW: the rack RESTS naturally on the white surface — its lowest points make solid physical contact with the ground, sitting firmly and stably. It is NOT floating, hovering, or suspended in mid-air. At EVERY point where the part touches down, render a soft, realistic contact shadow anchored right at that contact point — darkest and tightest exactly where the metal meets the surface, fading softly outward. Those grounded contact shadows are the only shadows in the image. Do NOT render a single detached, offset, or floating drop shadow beneath a hovering object.

COMPOSITION — CENTERED: center the entire rack horizontally and vertically within the frame, with even, balanced white space on all four sides. Do NOT push the subject to one side, corner, or edge. This is a framing/crop adjustment only — it does NOT change the camera angle, viewpoint, or perspective, which stay locked to the CAD.

LIGHTING: relight the part with rich, sculptural, premium studio lighting so every tube reads as strongly three-dimensional and round — a bright, crisp specular highlight ribbon along each tube crown falling off smoothly to a deeper, richer shadowed side, giving full roundness and form. This must NOT be flat, uniform, grey, or washed out. Keep a clean, bright, high-key feel with a soft key from above-front plus gentle fill, so recessed areas, inner-facing tubes, rear tubes, and the far side frame all stay readable with no muddy black holes — but allow real tonal range and genuine depth in the shadows rather than lifting everything to a flat grey. Punchy, dimensional, high-end: deep rich blacks, clean bright highlights, strong sense of form on every tube and plate.

RENDER QUALITY: photoreal, physically accurate materials, tack sharp, rich tonal contrast with deep true blacks and clean bright highlights, neutral true-to-life colour, subtle film grain, faint atmospheric depth, crushed blacks that retain shadow detail. Premium, punchy, and indistinguishable from a real high-end product photograph.
```

## Version B — Standard (tube only)

**12,179 characters**

```text
Turn the uploaded CAD render into a photorealistic studio product photograph of the same motorcycle pannier rack / side-case luggage carrier. This is a re-render of the exact image provided, not a new shot.

REFERENCE IMAGES: the main CAD render is the part to photograph.

═══════════════════════════════════════════════════════════════════════════
WHAT THIS PART IS — READ CAREFULLY BEFORE RENDERING
═══════════════════════════════════════════════════════════════════════════

This rack is made ALMOST ENTIRELY OF ROUND TUBING. It consists of:

• TWO large, open, rectangular/trapezoidal tubular side frames — big empty hoops you can see straight through
• Connecting cross tubes joining the two frames
• SPLIT CLAMP COLLARS at the ends of the lower support tubes — two-piece collars that wrap a tube and are pinched shut by small bolts
• A few small FLAT MOUNTING TABS and one narrow flat strap, each with one or two plain holes, bolted or welded at specific points

THAT IS ALL. There is NO large flat panel, NO big mounting plate, NO sheet-metal sidewall, and NO grid or array of holes anywhere on this product. Do NOT invent, add, or hallucinate any flat plate, panel, tray, or plate-with-many-holes. If you find yourself rendering a broad flat sheet surface, you are wrong — this part is tubes plus a handful of small tabs.

Also FORBIDDEN: adding small feet, nubs, pads, studs, buttons, or rivets along the bottom rails or anywhere on the tubes. Adding threaded rods, bolt shafts, or studs PROTRUDING or sticking up/out into the air. Every fastener sits tight and compact against its joint — nothing sticks out into open space.

═══════════════════════════════════════════════════════════════════════════
RULE ZERO — HARDWARE: THE SILVER TEST (HIGHEST PRIORITY)
═══════════════════════════════════════════════════════════════════════════

Hardware is identified by COLOUR in the CAD, not by the presence of holes. Real fasteners render in the CAD as small, discrete, BRIGHT SILVER / CHROME / GREY-METALLIC components — compact hex bolt heads, nuts, and thin washers — clearly distinct from the yellow painted tubes and tabs.

Apply this test to EVERY fastener before rendering it:

• Does the CAD show a small BRIGHT SILVER/CHROME fastener at this exact spot? → YES: render it.
• Is this spot just a HOLE — dark, empty, recessed, or the same colour as the surrounding metal? → NO HARDWARE. Render a clean, empty, open hole. Nothing in it. Ever.

THE PLAIN HOLES IN THE FLAT MOUNTING TABS AND THE TOP STRAP ARE EMPTY. They ship unfilled because the customer's own bolts go there at installation. A hole is NOT an invitation to add a bolt.

EXPLICITLY FORBIDDEN: adding a bolt to any plain tab hole or strap hole. Adding a fastener to "balance" or "match" another. Adding hardware for symmetry, completeness, or realism. If you cannot point to a bright silver fastener in the CAD at that exact spot, do not render one.

HARDWARE FINISH — ALWAYS STAINLESS STEEL: every fastener is polished STAINLESS STEEL — bright silver metallic with a clean, slightly reflective sheen and a crisp specular highlight, clearly distinct against the black powder coat. NEVER black, NEVER dark, NEVER powder-coated, NEVER dull zinc.

HARDWARE SIZE AND SHAPE — SMALL, COMPACT, CORRECT: reproduce each fastener at the exact modest scale shown in the CAD — small, neat hex bolt heads with thin flat washers and compact hex nuts, sitting tight and flush against their joint. Do NOT render fasteners oversized, chunky, bulbous, elongated, or blobby. Do NOT extend a bolt shaft into the air. Hex heads are crisp six-sided shapes with clean flats and sharp corners.

STRUCTURAL PARTS ARE ALWAYS BLACK: every tube, side frame, mounting tab, flat strap, bracket, and CLAMP COLLAR BODY is textured black powder coat — no matter how small or hardware-like it looks. The clamp collar bodies in particular are structural steel and are BLACK, not silver. Do NOT render any collar, tab, bracket, or strap in bare aluminium, raw metal, or stainless. The ONLY stainless items in the entire image are threaded fasteners: bolt heads, nuts, and washers. If it is a threaded fastener it is stainless; if it is structural metal it is black.

BEFORE FINISHING, AUDIT every fastener in your output. Confirm you can point to a bright silver fastener at that exact location in the CAD. Delete any you cannot. Ending with FEWER fasteners is a lesser error than adding even one that isn't there.

═══════════════════════════════════════════════════════════════════════════

CAMERA — MOST IMPORTANT GEOMETRY RULE: keep the exact same camera angle, viewpoint, orientation, rotation, perspective, and framing as the uploaded CAD render. Reproduce that identical view. Do NOT rotate, tilt, re-angle, zoom, recompose, or move the camera. Only render changes — render-to-photograph; the viewpoint is locked to the input.

PRESERVE PROPORTIONS — TRUE SHAPE, NO SQUISH: keep the part's true real-world proportions and aspect ratio exactly as in the CAD. Do NOT scale non-uniformly, stretch, squash, elongate, widen, compress, or foreshorten in any direction. The two rectangular side frames must render as FULL, LARGE, OPEN, correctly-proportioned hoops — never small, shrunken, squished, flattened, or narrowed — matching the true rectangle shape, size, and open airiness of the CAD. Present the whole rack at a generous, consistent size filling most of the frame with comfortable, even margins, scaled UNIFORMLY only.

CRITICAL — EXACT GEOMETRY, ADD NOTHING: reproduce the CAD's exact tubular structure — the same two open rectangular side frames, the same connecting cross tubes, the same clamp collars, and the same small flat tabs and strap, in the same positions and count. Keep that wide, open, airy structure. Do NOT compact or densify it. Do NOT turn it into crash bars, a box, a basket, or a cage. Do NOT invent, add, duplicate, or reshape any tube, tab, bracket, collar, plate, foot, or fastener. Every fitting maps one-to-one to a fitting in the CAD.

Pay special attention where tubes OVERLAP, CROSS, or PASS BEHIND one another — especially around the connecting cross tubes and where the frames meet the lower support arms. Render ONLY the tubes present in the CAD, with no phantom, echoed, doubled, or extra tubing anywhere. The total count of tubes and their exact paths must match the CAD one-to-one.

GEOMETRY: preserve every tube, bend, curve, junction, rectangular loop, clamp collar, flat mounting tab, flat strap, and hole exactly as shown, at the exact positions and proportions in the CAD. Keep tube diameters and bend radii identical. Add nothing, remove nothing, reshape nothing. Holes stay holes — reproducing a hole means rendering an empty opening, never filling it with a fastener.

MATERIAL — IGNORE THE CAD'S PLACEHOLDER COLOUR: the CAD uses yellow as a placeholder. In the real product EVERY structural component — all tubes, side frames, tabs, straps, brackets, and clamp collar bodies — is finished in ONE single uniform textured BLACK powder coat. There is no yellow, no two-tone, no colour difference between any parts.

The coating has a fine, even, sandy micro-grain across every surface — low gloss, roughly 15 gloss units, scattering light into soft broad highlights rather than sharp mirror reflections. Deep, rich, saturated neutral black with real depth — never washed out, grey, dull, or flat. No blue or brown cast. The grain must be clearly readable so it reads as a genuine powder-coated part, not a smooth or lifeless 3D surface. HIGHLIGHTS: a bright, crisp specular ribbon rides the crown of each round tube to reveal its round cross-section.

═══ WELDS — STRICT HIERARCHY, IN THIS ORDER OF PRECEDENCE ═══

RULE 1 — BOLTED JOINTS ARE NEVER WELDED (overrides everything below): if a joint has ANY fastener at it — bolt, nut, screw, or washer — that joint is BOLTED and gets absolutely NO weld bead. Not on it, not around it, not near it. A bolt and a weld are mutually exclusive. Every CLAMP COLLAR and every bolted tab is a BOLTED assembly — render its stainless hardware and leave that joint completely clean with no weld texture whatsoever. If you see hardware at a joint, do not weld it.

RULE 2 — WELDS APPEAR ONLY WHERE FLAT MEETS ROUND TUBE, WITH NO FASTENER: a TIG weld bead appears only where a flat tab, strap, or bracket is permanently fixed directly onto a ROUND TUBE with no fastener present. Slightly raised, evenly spaced stack-of-dimes ripples about 3mm wide, following the joint and catching a soft highlight.

RULE 3 — WELDED TUBE-TO-TUBE JUNCTIONS: where one tube is permanently welded directly to another tube with no fastener present, a continuous bead wraps that junction fully.

RULE 4 — NO FLAT-TO-FLAT WELDS: never add a bead where one flat component meets another flat component — tab to strap, bracket to bracket, collar to tab. A weld requires a ROUND TUBE on one side AND no hardware at the joint. If both sides are flat, there is no weld.

RULE 5 — NO MID-SPAN WELDS: no weld beads along the smooth straight or curved runs of any tube.

Summary: weld beads exist ONLY at fastener-free tube-to-tube junctions and fastener-free flat-to-round-tube joints. No bolted joints, no clamp collars, no flat-to-flat, no mid-span.

═══ BOLTED ASSEMBLIES — DISCRETE PIECES, NOT FUSED ═══

Where components are bolted together — the split clamp collars around tubes, the tabs to the frames — they are SEPARATE physical pieces clamped by hardware, not one continuous fused mass. Render each with its own visible outline and edges, a crisp parting line where they meet (the split collars have a visible seam between their two halves), a visible step in material thickness where one sits against another, and a compact stainless fastener visibly clamping them. Do NOT blend, melt, fillet, or flow one component into another.

BACKGROUND: a plain, solid, pure white background — completely empty and featureless. No studio, softbox, light tent, diffusion panels, walls, corners, seams, floor line, props, motorcycle, or visible lighting gear. Nothing but flat, even, seamless white. Clean white shows straight through both open rectangular side frames and every hole.

GROUNDING & CONTACT SHADOW: the rack RESTS naturally on the white surface — its lowest points make solid physical contact with the ground, sitting firmly and stably. It is NOT floating, hovering, or suspended in mid-air. At EVERY point where the part touches down, render a soft, realistic contact shadow anchored right at that contact point — darkest and tightest exactly where the metal meets the surface, fading softly outward. Those grounded contact shadows are the only shadows in the image. Do NOT render a single detached, offset, or floating drop shadow.

COMPOSITION — CENTERED: center the entire rack horizontally and vertically within the frame, with even, balanced white space on all four sides. Do NOT push the subject to one side, corner, or edge. This is a framing/crop adjustment only — it does NOT change the camera angle, viewpoint, or perspective, which stay locked to the CAD.

LIGHTING: relight the part with rich, sculptural, premium studio lighting so every tube reads as strongly three-dimensional and round — a bright, crisp specular highlight ribbon along each tube crown falling off smoothly to a deeper, richer shadowed side, giving full roundness and form. This must NOT be flat, uniform, grey, or washed out. Keep a clean, bright, high-key feel with a soft key from above-front plus gentle fill, so recessed areas, inner-facing tubes, rear tubes, and the far side frame all stay readable with no muddy black holes — but allow real tonal range and genuine depth in the shadows rather than lifting everything to a flat grey. Punchy, dimensional, high-end: deep rich blacks, clean bright highlights, strong sense of form on every tube.

RENDER QUALITY: photoreal, physically accurate materials, tack sharp, rich tonal contrast with deep true blacks and clean bright highlights, neutral true-to-life colour, subtle film grain, faint atmospheric depth, crushed blacks that retain shadow detail. Premium, punchy, and indistinguishable from a real high-end product photograph.
```
