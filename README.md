# xinhertz-hero-xray-test

**TEST ONLY playground** — 3D X-ray SOP-8 hero animation + diode cursor,
a concept for the xinhertz.top homepage hero.

This repo is intentionally separate from the live site
(`chipquay/chipquay.github.io`). Nothing here affects xinhertz.top.

## What is being tested

1. **3D SOP-8 chip** (Three.js, procedural model — real SOIC-8 proportions):
   slow auto-rotation + gentle float.
2. **X-ray on hover**: resting the cursor on the package fades the epoxy
   mold compound and reveals the internals — silicon die, gold wire bonds,
   copper leadframe — with part labels. Moving the cursor away restores the
   package. Nothing else on the page moves.
3. **Diode cursor**: the whole page uses a diode icon as the mouse cursor
   (made from a real diode product photo).
4. Mobile: tap the chip toggles X-ray. WebGL/CDN failure: static photo fallback.

## View it

https://chipquay.github.io/xinhertz-hero-xray-test/

## Files

- `index.html` — everything (inline CSS + module JS, Three.js via CDN)
- `assets/diode-cursor.png` / `assets/diode-cursor@2x.png` — cursor icons
- `assets/chip-photo.png` — fallback photo

## Next step (after user approval)

Port the approved version into the real homepage hero of
`chipquay.github.io` (scoped cursor, integrated with existing hero copy).
