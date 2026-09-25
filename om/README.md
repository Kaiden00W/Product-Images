# OM — Outback Motortek Product Prompts

The curated prompt library for Outback Motortek product imagery. These were refined over a year of
real generations. **Start from the matching prompt here; don't write a new one from scratch.**

**Model:** Nano Banana Pro, run on **Higgsfield**.
**House look:** textured black powder coat, polished stainless fasteners, on plain pure white, with
colourway recolours made from the approved black shot.

See [`house-style.md`](house-style.md) for the shared specs: colours, finishes, backgrounds, the OM
plaque, and the hardware and weld rules every prompt repeats.

---

## How the pipeline works

1. **CAD → Photo.** Upload the CAD render as Image 1 and use the product's prompt from `cad-to-photo/`.
   The result is the approved **black** product shot.
2. **Recolour.** Upload that approved black shot as Image 1 and use a prompt from `recolour/`. The
   camera, geometry, hardware, welds, lighting and background stay frozen, so only the paint changes.
3. **When a generation is wrong,** find the line that caused it and fix *that line*. Don't add a
   counter-rule, and don't start again.

**Upload order matters.** The prompts refer to "IMAGE 1", "IMAGE 2" and "the badge image", so
upload in the order each file lists.

---

## CAD → Photo

| Product | File | Extra uploads | Chars |
|---|---|---|---|
| Skid plate | [skid-plate.md](cad-to-photo/skid-plate.md) | — | 14.5k |
| Tail tidy / fender eliminator | [tail-tidy.md](cad-to-photo/tail-tidy.md) | OM badge | 5.7k |
| Crash bars — CAD screenshot | [crash-bars.md § A](cad-to-photo/crash-bars.md) | — | 13.7k |
| Crash bars — rendered CAD | [crash-bars.md § B](cad-to-photo/crash-bars.md) | OM badge (with add-on) | 5.5k (+1.1k) |
| Reckless rack (L+R arms) | [reckless-rack.md](cad-to-photo/reckless-rack.md) | OM badge | 7.1k |
| Pannier rack — with plates | [pannier-rack.md § A](cad-to-photo/pannier-rack.md) | — | 12.9k |
| Pannier rack — standard, tube only | [pannier-rack.md § B](cad-to-photo/pannier-rack.md) | — | 13.1k |
| Rear combo (rear rack) | [rear-combo.md](cad-to-photo/rear-combo.md) | — | 12.6k |
| Protection combo — V2 | [protection-combo.md](cad-to-photo/protection-combo.md) | — | 8.4k |
| Protection combo — V1 + plaque | [protection-combo.md](cad-to-photo/protection-combo.md) | OM badge | 8.7k |
| KTM protection combo (orange/black) | [ktm-protection-combo.md](cad-to-photo/ktm-protection-combo.md) | — | 17.8k |
| Luggage combo | [luggage-combo.md](cad-to-photo/luggage-combo.md) | — | 12.9k |

## Recolour (input: the approved black shot)

| Product → colourway | File | Background | Chars |
|---|---|---|---|
| Skid plate → white | [skid-plate-black-to-white.md](recolour/skid-plate-black-to-white.md) | #6B6B6B gradient grey, cinematic | 6.6k |
| LCB → signal red gloss | [lcb-black-to-red.md](recolour/lcb-black-to-red.md) | frozen (white) | 7.1k |
| UCB → red, top bracket black | [ucb-black-to-red.md](recolour/ucb-black-to-red.md) | frozen (white) | 9.7k |
| Crash bars → KTM orange two-tone | [crash-bars-black-to-orange.md](recolour/crash-bars-black-to-orange.md) | frozen (white) | 9.5k |
| PC → red, skid plate black | [pc-black-to-red.md](recolour/pc-black-to-red.md) | frozen (white) | 9.5k |
| UPC → red, top bracket + plate black | [upc-black-to-red.md](recolour/upc-black-to-red.md) | frozen (white) | 11.3k |
| Protection combo → white, plate black | [protection-combo-black-to-white.md](recolour/protection-combo-black-to-white.md) | #828282 mid grey | 8.7k |
| Crash bars → white (match reference) | [crash-bars-black-to-white-from-reference.md](recolour/crash-bars-black-to-white-from-reference.md) | dark charcoal from ref | 2.4k |

Abbreviations: **SP** skid plate · **LCB** lower crash bars · **UCB** upper crash bars ·
**PC** protection combo · **UPC** upper protection combo.

---

## New OM product?

1. Pick the closest existing prompt by construction: folded sheet → skid plate. Tubes →
   crash bars. Tubes plus flat plate → rear combo or luggage combo. Two separate pieces →
   protection combo.
2. Copy it and change the **product name** and the **structure description**.
3. **Re-derive every count and every named feature from the new CAD.** Many of these prompts
   hard-code facts about their own part: three weld nuts, three castle prongs, one rear mount
   bracket, "at most three" weld gaps. A carried-over count makes the model invent or delete
   features to hit it.
4. Keep the shared blocks word-for-word from [`house-style.md`](house-style.md).
5. Once it works, save it here as a new file and add a row to the table above.

## About length

The generic skill says fidelity prompts work best at 3–6k characters. Most of these are 8–18k
because each paragraph was added to fix a real failure on that part. Treat them as proven. If you
trim one, run the trimmed and original versions side by side on the same CAD before replacing it.
