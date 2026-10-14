# 🎨 JAMM Pad — Joint Art & Modeling Machine

A retro paint studio in **one single HTML file**. No install, no account, no internet required. Draw with a **mouse, touch screen, or game controller** — and let the built-in **AI Painter** create art for you, completely offline.

## ⬇️ Get it (pick any — free, no signup)

| How | Where |
|---|---|
| **Easiest — one-click download** | 👉 **[Download jamm-pad.html](https://github.com/JAMMx2/jamm-pad/releases/latest/download/jamm-pad.html)** 👈 then double-click the file. Done — works forever, zero internet. |
| **Play online** (installable) | **https://jammx2.github.io/jamm-pad/** — keeps working offline after your first visit |
| **From the live app** | Press the **Download App** button in the toolbar |
| **Whole repo** | Green **Code** button → **Download ZIP** → open `index.html` |

> **If the downloaded file opens in a text editor:** right-click it → **Open with** → Chrome / Edge / Firefox / Safari.

## ✨ AI Painter — type an idea, get art (100% offline)

Open the panel (or press the **AI Paint** button), type something like:

- `sunset mountains, calm`
- `neon city at night`
- `galaxy with a ringed planet`
- `pastel flower garden`
- `aurora over snowy forest`
- `rainbow mandala, detailed`
- `erupting volcano at night`
- `snowy village, glowing windows`
- `pastel hot air balloons at sunrise`

…and watch it get **painted stroke by stroke on a new layer**. The built-in art brain understands **subjects** (mountains, ocean, forest, city, village, volcano, balloons, space, flowers, mandala, aurora, underwater, desert, abstract), **palettes** (warm, pastel, neon, vaporwave, ice, mono, rainbow…), **colors**, and **moods** (calm, chaotic, minimal, detailed, misty, glowing, night…).

- **Variation** = same idea, brand-new take. **Surprise** = random idea.
- Every image is unique and seeded — no internet, no APIs, no accounts, and your prompts never leave your device.
- Results land on their own layer, so paint over, erase, or remix freely.

## 📦 Import & export art

- **Export .jam** — saves your whole artwork (all frames, all layers, names, opacity, fps) as one portable file. Share it, back it up. v1.1 `.jam` files still open.
- **Import** — open a `.jam` to continue where you left off, or import **any image (PNG/JPG)** as a new layer to paint over.
- **Save PNG** — flatten and export at **1x, 2x or 4x** (crisp nearest-neighbour scaling), with or without the white paper (**Transparent**).
- **Export GIF** — every animation frame as a looping animated GIF, encoded in-page (no libraries, no upload).
- **Sprite sheet** — all frames side by side in one PNG, at the same 1x/2x/4x scale.
- **Autosave** — your work is written to the browser (IndexedDB) a few seconds after each change. A **Restore autosave** button appears in the Projects panel next time you open the app.
- Quick-save projects also live in your browser via the Projects panel.

## 🖌 Features

- **Animation** — frames with their own layers, duplicate / blank / delete, onion skin of the previous frame, play/stop at 1–24 fps, GIF + sprite-sheet export. `,` and `.` step frames.
- **Layers** with opacity, visibility and reordering.
- **Tools**: pen, eraser, line, rect, ellipse, polygon, flood fill (with a **tolerance** slider), gradient fill, color picker, spray, select / move / copy / paste, and a **Text** tool (Sans / Serif / Mono, bold).
- **Pixel-art mode** — toggle **Pixel grid**: a grid overlay plus snapping for every tool, with clean whole-cell shapes and lines (2–32 px cells).
- **Pen pressure** — stylus pressure drives brush size (PointerEvent pressure; toggle in Tool options).
- **Palette editor** — add / remove swatches, reset, and **import / export GIMP `.gpl` or plain `.hex`** lists. Your palette is remembered on the device.
- Radial **symmetry** (1–16) + mirror, glow / sketch / rainbow brush modes, brush styles (round, flat, marker, pixel).
- Effects (blur, pixelate, gray, sepia, lighter, darker), flip / rotate / invert, reference image underlay, **timelapse replay**, zoom + pan.
- Undo / redo (Ctrl+Z, Ctrl+Y, Ctrl+Shift+Z) that survives adding, deleting and reordering layers.
- Single-key tool shortcuts (`P E L R O Y F G I A M T`), `X` swaps colors, `Esc` cancels.
- Full **game controller support** (draw with a PS/Xbox pad).

Press **Controls** in the app (or `H`) for every shortcut.

## 📴 How offline works

Everything lives in one self-contained HTML file — zero external requests, ever.

- **Downloaded copy:** works from your disk forever. AI Painter included.
- **Online version:** a service worker caches the app on first visit, so it loads and works with no connection, and your browser will offer to **install it like an app** (icon, own window).

## 🔒 Privacy

No analytics, no tracking, no network calls. Art and prompts stay on your device.

## License

MIT © 2026 Christopher Moore
