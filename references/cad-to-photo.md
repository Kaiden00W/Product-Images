# CAD → Photoreal Product Photograph

## THE BASE TEMPLATE (~3,300 chars — start here)

This is the version that finally worked first-try after a long chain of bloated
failures. Adapt the part name and the material. Resist adding to it.

```
Turn the uploaded CAD render into a photorealistic studio product photograph of the
same motorcycle [PART]. This is a re-render of the exact image provided, not a new shot.

CHANGE NOTHING ABOUT THE PART. Reproduce the exact same camera angle, viewpoint,
perspective and framing as the upload. Reproduce every panel, fold, facet, side wall,
bracket, slot, hole and cut-out exactly as shown, in the same shapes, positions and
counts. Add nothing, remove nothing, reshape nothing, simplify nothing. The only thing
that changes is CAD-to-photograph.

MATERIAL: laser-cut aluminium sheet, press-brake folded, finished in a textured black
powder coat. The coating has a fine, even, sandy micro-grain across every surface — low
gloss, roughly 15 gloss units, scattering light into soft broad highlights rather than
sharp reflections. Deep, rich, neutral black with real depth. The grain reads clearly so
it looks like genuine powder-coated metal, not a smooth 3D surface. The CAD's colour is a
placeholder — the real part is black.

HARDWARE: reproduce only the fasteners actually visible in the CAD, in the same positions
and the same quantity. Do not add a bolt, nut or washer anywhere the CAD does not show
one — every slot, hole and cut-out is open and empty, and a hole is never an invitation
for a fastener. Every fastener is polished stainless steel: bright silver metallic with a
crisp specular highlight, clearly distinct against the black coat. They are small M8
hardware, neat and compact, sitting flush — not chunky or oversized. Everything that is
not a threaded fastener is black powder coat, including brackets, tabs, spacers and sleeves.

WELDS: TIG weld beads appear only where the edges of two separate panels meet — the seams
where one piece of plate joins another. Each is a slightly raised stack-of-dimes bead
running the length of that seam, welded solid so no gap or light shows through. The part
is welded first and coated afterwards, so every bead is the same textured black as the
panels — visible as raised rippled texture, never bare metal.

Where a single sheet simply folds to change direction, there is no weld — just a clean
radiused bend with a crisp specular line along the crest. Folds are not seams.

BACKGROUND: a plain, solid, pure white background — completely empty and featureless. No
studio, softbox, walls, seams, floor line or props. Clean white shows through every slot,
hole and cut-out. The part rests solidly on the surface with a soft contact shadow directly
beneath it, tight where the metal meets the surface and fading outward. That shadow is the
only thing on the white besides the part.

LIGHTING: bright, clean, high-key product lighting that reaches every recessed and interior
face with no muddy dark pockets, while keeping real tonal separation between facets so each
folded plane sits at a different brightness and the geometry reads strongly
three-dimensional. Deep blacks in the shadowed planes, clean highlights on the up-facing
planes, a crisp specular line on every fold.

RENDER QUALITY: photoreal, physically accurate materials, tack sharp, rich tonal contrast
with deep true blacks, neutral true-to-life colour, subtle film grain. Indistinguishable
from a real high-end product photograph.
```

---

## RULE SETS TO ADD **ONLY** WHEN THE BASE FAILS

Add one at a time. Never all of them.

### Hardware identified by SHAPE, not colour
Needed when the CAD is monochrome (all grey, all orange). The "look for bright
silver" test returns nothing and fasteners get painted body-colour.

```
DO NOT USE COLOUR TO FIND HARDWARE. The CAD is rendered in one flat placeholder
colour, so fasteners are not distinguished by being silver. Identify them by SHAPE.

A FASTENER is ONLY one of these: a HEX NUT, a HEX BOLT HEAD, a WASHER, or a length of
EXPOSED THREADED SHAFT. NOT FASTENERS — these are structural and painted: cylindrical
spacers and sleeves, clamp collars, brackets, mounts, tabs, flanges and plates. A
cylindrical sleeve is not a bolt. A clamp collar is not hardware. Anything bigger than a
nut that is not itself threaded is painted.
```

### Hardware count from the CAD, not from a number
**Never hard-code a count** unless the CAD is in front of you, and mark it if you do.
A stale "exactly three" converted three X-shaped cut-outs into three nuts.

```
COUNT FROM THE CAD: count the fasteners genuinely visible from this viewpoint and render
exactly that many, in exactly those positions. One hidden behind a bracket stays hidden.
Do not work to a target number.
```

### Hardware size
Chronic failure: M8 nuts rendered at roughly M12.

```
SIZE — TINY: roughly M8, about 13mm across the flats, on a part several hundred
millimetres long. Small, quiet, incidental details. If a nut or bolt head reads as a
prominent, eye-catching shape, it is FAR too large — shrink it.
```

### Camera lock (the no-new-surfaces test)
Needed when the model re-shoots to a more flattering angle.

```
THE NO-NEW-SURFACES TEST: compare your output to the CAD — can you see any face, panel
or surface that was NOT visible in the CAD? If yes, the camera moved and the render is
WRONG. The same surfaces are visible, at the same angles, showing the same amount of each.

COMPOSITION — A CROP, NEVER A RE-SHOOT: you may present the part larger than the CAD
does, but this is a pure crop and zoom of the identical photograph. If making it bigger
would require seeing more of the part, do not make it bigger. Matching the CAD's angle
always beats filling the frame.
```
⚠️ Any "fill most of the frame" wording MUST be subordinated to this or it re-shoots.

### CAD viewport artifacts
For screenshots rather than finished renders — faint facet and body-split lines get
read as weld seams.

```
The upload is a CAD viewport screenshot containing display artifacts that are NOT
physical features: faint segment, tessellation and facet lines on the surfaces; body
split lines where separate CAD bodies meet; mesh edges and patch boundaries. IGNORE ALL
OF THESE. A line in the CAD is not evidence of a weld.
```

### Crowded junctions (tubular parts)
For crash bars / racks where tubes cross and fuse into a lump.

```
Where tubes cross, converge or pass behind one another, resolve the DEPTH ORDER — one
tube in front, one behind, the front cleanly occluding the other with a clear dark
separation. Never let two tubes blend, merge or fuse. Every tube stays complete,
continuous and round through the region, at constant diameter. Do not simplify a busy
area into a blobby mass, omit a small part, or add phantom or doubled tubing.
```

### Split clamp collars
They render as open forks with a bolt floating in air.

```
Each tube-end clamp is a SPLIT CLAMP COLLAR: a complete ring of metal FULLY ENCIRCLING
the tube, two halves meeting at a pair of flat bolt ears. The band wraps a FULL 360
DEGREES — closed and unbroken, no gap or missing section. Both bolt ears present, with a
stainless bolt through BOTH and a nut on the far side. A crisp parting line across the
ears. THE BOLT ALWAYS PASSES THROUGH SOLID METAL — never floating in open air.

NEVER an open C-shape, half ring, horseshoe, fork, prongs or a collar with one side
missing. A clamp is a machined collar with real wall thickness — never describe it as a
"band" or "strap", which produces hose-clamp ribbons.
```

### No mirroring or duplication
The model invents symmetry — it duplicated a rear mount into a mirrored twin.

```
Count every bracket, mount, tab and lug and render EXACTLY that many. This assembly is
NOT symmetrical and must not be made symmetrical. If the CAD shows a feature on one side
only, it exists on one side only. Never add a mirrored twin for balance, and never delete
a feature because the other side lacks one.
```

### Bolt thread through a nut
Where the CAD shows a bolt threaded up through a weld nut with its cut end proud.

```
Where the CAD shows a bolt threaded through a nut with its cut end standing proud above
the nut's top face, reproduce that — a short cylindrical stub of visible thread roughly
2 to 4mm above the nut, with the bore FILLED by the bolt. Where the CAD shows a bare nut,
leave the bore open.
```
⚠️ Never write a blanket "no shaft protruding" rule — it deletes this.

---

## FEATURE PRESERVATION — generic, safe to reuse across parts

Prefer these over naming a specific part's features, so the prompt stays portable.

```
• Every SLOT GROUP — same number, spacing, length and angle. Do not thin out, add to or
  redistribute a group.
• Every CUT-OUT — reproduce its exact shape. A cross stays a cross, a kidney stays a
  kidney. Never round a shaped cut-out into a circle and never fill one in.
• Every BRACKET AND MOUNT — reproduce its true outline including curved, stepped or
  scalloped edges. Do not simplify a shaped bracket into a plain flat tab.
• Any SEPARATE OVERLAID PLATE stays readable as a distinct second sheet on top of the one
  below, with its own outline, edge and a visible step in material thickness.
• Holes stay holes — an empty opening with a crisp cut edge and visible sheet thickness at
  the rim, never filled with a fastener.
```
