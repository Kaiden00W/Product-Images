# Skid Plate — CAD → Photo

Folded aluminium bash plate, textured black powder coat, on pure white.

**Model:** Nano Banana Pro on Higgsfield  
**Upload:** Image 1: the CAD render (orange placeholder colour).

### Before you paste

- **This prompt is written for one specific skid plate.** It hard-codes *exactly three M8 weld nuts* on the flat rear mounting plate, a plate *over 400mm long*, *at most three* weld gaps, a *cylindrical spacer* on the rear bracket and *two upright brackets*. For a different skid plate, recount every one of these against its CAD before sending. A wrong count makes the model invent or delete features to hit it.

### What this prompt is guarding against

- Nuts rendered at M12 size instead of M8 → absolute size + 1/30th ratio + "if you notice it first, it's too big" test
- Bolts/washers invented in the side-wall holes and on the spacer → named zero-hardware zones
- Every fold welded → "start at zero, earn each bead" + the open-gap test + hard ceiling of three
- Weld nuts turned into bolted joints → explicit "what a weld nut is" list

---

## Prompt

**12,506 characters**

```text
Turn the uploaded CAD render into a photorealistic studio product photograph of the same motorcycle skid plate. A re-render of the exact image provided, not a new shot.

╔═════════════════════════════════════════════════════════════════════════╗
║  THE SIX ABSOLUTE RULES — OBEY THESE ABOVE EVERYTHING ELSE              ║
║                                                                         ║
║  1. EXACTLY THREE silver objects exist in this image. All three are     ║
║     WELD NUTS on the flat rear mounting plate. A fourth silver object   ║
║     anywhere is a failure.                                              ║
║                                                                         ║
║  2. THE NUTS ARE M8 — TINY. 13mm across the flats, on a plate over      ║
║     400mm long. Each nut is about 1/30th of the plate's length. If a    ║
║     nut reads as a prominent feature of the photograph, it is FAR too   ║
║     big. They are small details you have to look for.                   ║
║                                                                         ║
║  3. DO NOT MOVE THE HARDWARE. Same spots as the CAD, same spacing.      ║
║                                                                         ║
║  4. START WITH ZERO WELD BEADS. Maximum THREE beads in the entire       ║
║     image. Four or more is a failure. A FOLD IS NEVER A WELD.           ║
║                                                                         ║
║  5. EVERY hole, slot and vent on this part is OPEN and EMPTY.           ║
║                                                                         ║
║  6. The part is BLACK. The orange in the CAD is a placeholder.          ║
╚═════════════════════════════════════════════════════════════════════════╝

═══════════════════════════════════════════════════════════════════════════
WELDS — START AT ZERO AND EARN EACH ONE
═══════════════════════════════════════════════════════════════════════════

This plate is PRESS-BRAKE FOLDED from continuous sheet metal. Begin by assuming it has NO visible weld beads anywhere at all. Do not add a single bead unless it passes the gap test below.

A FOLD IS NEVER A WELD. Every line where the sheet simply changes direction is a press-brake BEND: a clean, smooth, RADIUSED corner with the metal flowing continuously around it and a bright specular line riding the crest. NO bead. NO ripples. NO stitch texture. NO seam line. NO groove. The overwhelming majority of lines on this part are bends and get absolutely nothing.

Specifically, these all get NO weld bead:

• Every crease between two angled facets of the V-shaped shield
• Every fold where a side wall rises off the base
• The long top edges of the side walls
• Every cut edge and every outline
• The edges of the flat rear plate
• Any faint line, facet boundary, tessellation edge or body-split line in the CAD

THE GAP TEST — the only thing that earns a bead: the CAD must show an actual OPEN GAP at that spot — a visible dark slot of empty space between the edges of two genuinely separate pieces of metal, wide enough to see into. Not a line. Not a crease. Not a shading change. Not a facet boundary. An actual open gap.

HARD CEILING: there are AT MOST THREE such gaps on this entire part. If your output contains four or more weld beads, it is wrong — delete every bead and restart from zero.

Where a bead does belong, it sits DOWN IN the gap, filling it: slightly raised, tightly rippled stack-of-dimes about 3mm wide, crisp and controlled, never puffy, swollen, melted or rubbery.

The only other permitted welds are small tight fillets at the base of each weld nut and at the base of the cylindrical spacer — nowhere else.

═══════════════════════════════════════════════════════════════════════════
HARDWARE — THREE WELD NUTS, NOTHING ELSE
═══════════════════════════════════════════════════════════════════════════

Hardware is TRANSCRIBED from the CAD, never chosen. Three things are fixed and none may deviate: the COUNT, the POSITION, and the TYPE.

THE COMPLETE LIST: three WELD NUTS, clustered together on the FLAT REAR MOUNTING PLATE near the upright brackets. That is every fastener on this product. Nothing else on this part is a fastener and nothing else is silver.

WHAT A WELD NUT IS — render it exactly this way:

• A plain six-sided hex nut sitting DIRECTLY and FLUSH on the plate surface.
• With an OPEN, EMPTY, UNFILLED BORE through its centre — you see straight down the hole to the plate. It is captive hardware awaiting the customer's bolt.
• With a small tight weld fillet where its base meets the plate.
• NO bolt through it. NO bolt head on top. NO washer under it or on it. NO flange, NO integral washer face, NO serrated base, NO nylon insert collar. NO shaft, stud or shank protruding either way. NO domed cap. A weld nut is ONE captive component with an empty hole in the middle. That is all it is.

DO NOT convert it into a bolted joint. DO NOT add a washer — there are NO washers anywhere on this product. DO NOT render it as a nut clamping two pieces together.

═══ HARDWARE SIZE — THEY ARE M8 AND THEY ARE TINY ═══

This is the single most common error on this part. The nuts keep coming out roughly M12 when they should be M8. Get the scale right.

ABSOLUTE SIZE: each nut is a standard M8 hex nut — approximately 13mm across the flats and about 6.5mm tall. Small, neat, compact.

SIZE RELATIVE TO THE PART: this skid plate is over 400mm long. Each nut is therefore roughly ONE THIRTIETH of the plate's overall length. In the photograph they are small, quiet, discreet details — the kind of thing you have to look for, not the kind of thing you notice first.

THE TEST: if a nut reads as a prominent, eye-catching feature of the image, it is FAR too large — shrink it. If the three nuts together dominate or draw the eye away from the plate itself, they are far too large. When correct, the plate reads as the subject and the nuts are minor incidental detail on it.

Reproduce each fastener at the exact modest scale shown in the CAD, sitting tight and flush against the plate. Do NOT render them oversized, chunky, bulbous, blobby, thick, tall, or heavy-duty. Hex nuts are crisp six-sided shapes with clean flats and sharp corners at a small, correct, realistic scale.

═══ HARDWARE POSITION — DO NOT MOVE THEM ═══

Each weld nut sits at the EXACT spot on the rear plate that the CAD shows, in the same spatial relationship to the plate edges, the bracket, and to each other. Reproduce their spacing and their arrangement one-to-one. Do NOT redistribute them, re-space them evenly, spread them out, cluster them tighter, shift them along the plate, or rearrange their pattern. Their positions are copied, not composed.

ZERO-HARDWARE ZONES — hard count of zero, no exceptions:

• THE SIDE WALLS AND EVERY ROUND HOLE IN THEM — plain, empty, open, see-through. Nothing in them, nothing beside them. Hardware was wrongly invented here before; check it specifically.
• THE CYLINDRICAL SPACER on the rear bracket — a WELDED STEEL SLEEVE, powder coated black, NOT hardware. Its bore is open and empty. No bolt, nut, washer or cap on or near it. Hardware was wrongly invented here before; check it specifically.
• THE TWO UPRIGHT BRACKETS AND THEIR ELONGATED SLOTS — open, empty.
• THE RECTANGULAR VENT SLOTS in the side walls — open, empty.
• THE ENTIRE FOLDED SHIELD BODY, its underside, leading edge and every facet — completely bare.

THE TEST for any fastener: can I point to a distinct BRIGHT SILVER solid at this exact spot in the CAD? Anything else — a dark hole, a slot, a recess, a see-through shape, or a shape the SAME ORANGE as the surrounding metal — means NO fastener. Render an open empty hole or bare black metal.

FORBIDDEN: adding a fastener because a hole exists; putting hardware on a side wall, vent, bracket slot, spacer or the shield body; adding washers; adding a fastener to balance, mirror, pair or complete another; mirroring hardware between sides; adding hardware for symmetry or realism. If you feel an urge to add or upgrade a fastener you cannot point to in the CAD, that urge is the error.

NEVER OMIT: all three weld nuts must appear, in their exact positions.

FINISH: the weld nuts are bright silver stainless with a crisp specular highlight against the black coat. Every other component — every panel, fold, flange, side wall, bracket, spacer, tab and the rear plate — is textured black powder coat, no matter how small or hardware-like it looks.

═══════════════════════════════════════════════════════════════════════════
CAMERA AND GEOMETRY
═══════════════════════════════════════════════════════════════════════════

Keep the exact same camera angle, viewpoint, orientation, rotation, perspective and framing as the CAD. Do NOT rotate, tilt, re-angle, zoom, recompose or move the camera. Keep true proportions and aspect ratio — no non-uniform scaling, stretching or squashing.

Preserve every panel, fold, facet, side wall, cut-out, vent slot, hole, slot, flange, tab, bracket and boss exactly as shown: the folded V-shaped shield with its faceted underside and curved swept leading edge; the raised side walls with their stepped notched top profiles; the vent slots at the same count and spacing; the two upright rear brackets each with a pair of elongated slots; the pivoting linkage bracket with its cylindrical welded spacer and open bore; the flat rear plate and its extension tabs.

Add nothing, remove nothing, reshape nothing. Holes stay holes — an empty opening, never filled with a fastener. Keep sheet-metal thickness visible at every cut edge so panels read as real folded plate.

═══════════════════════════════════════════════════════════════════════════
MATERIAL, LIGHT AND FRAME
═══════════════════════════════════════════════════════════════════════════

MATERIAL: the CAD's ORANGE is a placeholder — the real part is NOT orange. Laser-cut aluminium sheet, press-brake folded, in ONE uniform textured BLACK powder coat with a fine even sandy micro-grain clearly readable across every face. Low gloss, roughly 15 gloss units. Deep rich neutral black, no blue or brown cast. Gritty and granular up close — not flat plastic, vinyl or a smooth 3D surface. A crisp specular line rides every fold and cut edge.

BACKGROUND: plain solid pure white, completely empty and featureless — no studio, softbox, panels, walls, seams, floor line or props. Genuinely white and evenly lit. Clean white shows through every slot, hole and weld-nut bore.

GROUNDING: the plate rests solidly on the surface in firm contact, not floating. A soft contact shadow anchored where metal meets surface, darkest at contact, fading outward. The only shadow in the image.

COMPOSITION: centred, at a generous size filling most of the frame with even margins, cropping nothing. Framing only — the camera angle stays locked to the CAD.

LIGHTING: bright, clean, high-key product lighting reaching every recessed, concave, vertical and interior face with no dark pockets — but NOT flat. Keep real tonal separation between facets so each folded plane sits at a different brightness and the geometry reads strongly three-dimensional. Deep blacks in shadowed planes, clean highlights on up-facing planes.

RENDER QUALITY: photoreal, tack sharp, crisp edges, rich contrast, deep true blacks, neutral colour, subtle film grain, fully resolved fine detail. Indistinguishable from a real studio product photograph.

═══════════════════════════════════════════════════════════════════════════
FINAL AUDIT — COUNT, DO NOT ESTIMATE
═══════════════════════════════════════════════════════════════════════════
1. COUNT the silver objects. The answer must be exactly 3, all on the rear plate. Delete any others.
2. MEASURE a nut against the plate. Its width must be about 1/30th of the plate's length. If it is bigger than that, shrink it until it is. If it catches your eye before the plate does, it is too big.
3. CHECK each nut is a plain hex nut — no flange, no washer face, no bolt, open empty bore.
4. CHECK the nuts sit in the same positions and spacing as the CAD, not redistributed.
5. COUNT the weld beads. If the answer is more than 3, delete every bead and restart at zero.
6. Look at every FOLD and facet crease — each must be a clean radiused bend with no bead.
7. Look at the SIDE WALL holes — open and empty, nothing in or beside them.
8. Look at the CYLINDRICAL SPACER — bare black metal, no fastener.
9. Confirm the part is black, not orange, and the powder coat grain is visible.
```
