# Changelog

All notable changes to JAMM Pad. The app is a single `index.html`; versions are shown in the title bar.

## 1.2.0 — 2026-10-13

### Added
- **Animation frames** — each frame carries its own layer stack. Duplicate (+), Blank, Delete, previous/next (`,` / `.`), onion skin of the previous frame, Play/Stop at 1–24 fps.
- **Animated GIF export** — pure-JS GIF89a writer (popularity palette, 256 colours per frame, LZW), no external code.
- **Sprite sheet export** — all frames in one horizontal PNG strip.
- **PNG export at 1x / 2x / 4x** (nearest-neighbour, pixel-crisp) and an optional **transparent** background.
- **Autosave** to IndexedDB a few seconds after each change, with a *Restore autosave* button on next launch.
- **Palette editor** — add the Left colour, remove, reset; **import / export GIMP `.gpl` and plain `.hex`** lists. Palette persists on the device.
- **Text tool** — click to place; Sans / Serif / Mono, bold; size follows the Size slider; honours symmetry, flow and glow.
- **Pixel-art mode** — grid overlay and snapping for every tool (2–32 px cells); lines, rects and ellipses are rasterised as whole cells.
- **Pen pressure** — stylus pressure scales the brush (PointerEvent `pressure`), toggle in Tool options.
- **Flood fill tolerance** slider (0–160).
- **Three new AI Painter scenes**: volcano, hot-air balloons, snowy village (plus new Surprise prompts).
- Keyboard: single-key tool shortcuts (`P E L R O Y F G I A M T`), `X` swap colours, `Esc` cancel, `Ctrl+Shift+Z` redo.
- Version tag in the title bar and Controls overlay.

### Changed
- `.jam` files are now **v2** (frames + fps). v1 files still import; v2 exports also keep a top-level `layers` entry so v1 readers get the first frame.
- Service-worker cache bumped to `jamm-pad-v3` so installed PWAs pick up the update.
- Layer thumbnails are rendered from a small canvas instead of encoding the full 1280x800 layer each refresh (much faster undo / layer switching).

### Fixed
- Flood fill could loop forever when the fill colour was within tolerance of the target colour (no visited mask). Now uses a visited mask and index-based stack.
- Undo / redo entries pointed at the wrong layer after adding, deleting or reordering layers (could throw on a deleted index). Indices are remapped and clamped.
- Loading a project with an empty layer list never finished; now guarded.
- Layer ops now commit a floating selection first instead of dropping it.
- Removed a dead `Calligraphy` style branch.

## 1.1.1
- Scene polish: edge fill, window placement, denser mandalas.

## 1.1.0
- Offline AI Painter, `.jam` import/export, accessibility polish.

## 1.0.0
- First release: single-file offline paint app, PWA, download button.
