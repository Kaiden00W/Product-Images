# Product-Images

The skill is named `product-image-prompts`; clone it into a folder with that name so
`/product-image-prompts` works in Claude Code.

A Claude Code skill for writing prompts for AI image and video generation —
Nano Banana Pro, Kling, Veo, Seedance, Higgsfield and similar.

- **Fidelity mode** — CAD renders → product photos, recolouring, exact logo reproduction
- **Creative mode** — ads, hero images, lifestyle/marketing imagery, short video

## Contents

| File | Purpose |
|---|---|
| `SKILL.md` | Core rules, mode selection, pre-flight checklist, workflow |
| `references/cad-to-photo.md` | CAD → photoreal product photograph |
| `references/recolour.md` | Colour changes on existing renders |
| `references/ads-and-lifestyle.md` | Ads, hero images, lifestyle shoots |
| `references/lighting.md` | Exposure, backgrounds, grounding, lighting |
| `references/video.md` | Kling / Veo / Seedance video prompts |
| `INSTALL.txt` | Step-by-step install guide |

## Install

Clone straight into your Claude Code skills folder:

```bash
# macOS / Linux
git clone https://github.com/Kaiden00W/Product-Images.git ~/.claude/skills/product-image-prompts

# Windows (PowerShell)
git clone https://github.com/Kaiden00W/Product-Images.git "$env:USERPROFILE\.claude\skills\product-image-prompts"
```

Restart Claude Code, then try: `write me a nano banana prompt for a jet ski rental ad`
or call it directly with `/product-image-prompts`. See `INSTALL.txt` for the manual steps.
