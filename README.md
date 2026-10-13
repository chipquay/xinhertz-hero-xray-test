# xinhertz-hero-xray-test

**TEST ONLY playground** — flat SOP-16 hero reveal + MLCC cursor,
a concept for the xinhertz.top homepage hero.

This repo is intentionally separate from the live site
(`chipquay/chipquay.github.io`). Nothing here affects xinhertz.top.

## What is being tested (v3, 2026-10-13)

Per the user's mockup: everything is **flat**, like a product photo.

1. **SOP-16 chip** (Three.js, procedural model — real SOIC-16 proportions,
   marked `74HC595D`), viewed near top-down, lying still.
2. **Reveal on hover**: sliding the cursor across the package crossfades the
   laser marking into the identity text **"Xinhertz — NXP Distributor"**
   printed flat on the mold compound (red, like the mockup). Moving the
   cursor away restores the original marking. Nothing else on the page moves.
   (v1: X-ray internals — removed. v2: glowing billboard text — replaced.)
3. **MLCC cursor**: AI-generated MLCC chip-capacitor icon at the same 3/4
   tilted angle as the user's reference photo, applied site-wide.
4. Mobile: tap the chip toggles the reveal. WebGL/CDN failure: static photo fallback.

## View it

https://xinhertz.top/xinhertz-hero-xray-test/

## Files

- `index.html` — everything (inline CSS + module JS, Three.js via CDN)
- `assets/mlcc-cursor.png` — cursor icon (AI-generated, 3/4 angle)
- `assets/media-generation-mlcc-angled-*.png` — cursor source render
- `assets/chip-photo.png` — fallback photo (74HC595D)

## Next step (after user approval)

Port the approved version into the real homepage hero of
`chipquay.github.io` (scoped cursor, integrated with existing hero copy).
