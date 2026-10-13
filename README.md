# xinhertz-hero-xray-test

**TEST ONLY playground** — 3D SOP-16 hero reveal + MLCC cursor,
a concept for the xinhertz.top homepage hero.

This repo is intentionally separate from the live site
(`chipquay/chipquay.github.io`). Nothing here affects xinhertz.top.

## What is being tested (v2, 2026-10-13)

1. **3D SOP-16 chip** (Three.js, procedural model — real SOIC-16 proportions,
   marked `74HC595D`): slow auto-rotation + gentle float.
2. **Reveal on hover**: sliding the cursor across the package fades the epoxy
   mold compound and the identity **"Xinhertz — NXP Distributor"** shines
   through from inside the chip (glowing billboard text). Moving the cursor
   away seals the package shut again. Nothing else on the page moves.
   (v1 showed internal die/wire-bond structure — removed per user request.)
3. **MLCC cursor**: the whole page uses an AI-generated MLCC chip-capacitor
   icon as the mouse cursor (user's MLCC photo was reference only).
4. Mobile: tap the chip toggles the reveal. WebGL/CDN failure: static photo fallback.

## View it

https://xinhertz.top/xinhertz-hero-xray-test/

## Files

- `index.html` — everything (inline CSS + module JS, Three.js via CDN)
- `assets/mlcc-cursor.png` — cursor icon (AI-generated)
- `assets/media-generation-mlcc-raw-*.png` — cursor source render
- `assets/chip-photo.png` — fallback photo (74HC595D)

## Next step (after user approval)

Port the approved version into the real homepage hero of
`chipquay.github.io` (scoped cursor, integrated with existing hero copy).
