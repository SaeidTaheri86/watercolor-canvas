# Drawing Canvas UI

A lightweight, browser-based drawing canvas with a physical instrument toolbar. Built with React, HTML Canvas, and Tailwind CSS — no build step required.

## Features

### Toolbar

| Section | What's there |
|---|---|
| **T** | Text tool — click anywhere on the canvas to place editable text, `Enter` to commit, `Esc` to cancel |
| **Tools** | Eraser, Pen, Pencil, Marker, Fine liner, Brush, Watercolor — all rendered as physical SVG instruments floating above the bar |
| **Color wheel** | Full HSL wheel — click or drag to pick any color, current color shown as center dot |
| **Swatches** | 6 circular presets in a 2×3 grid (navy, purple, crimson, gray, cyan, off-white) |
| **Size** | 4 dot sizes stacked vertically on the far right |

### Drawing Tools

| Tool | Behavior |
|---|---|
| **Pen** | Smooth, thin strokes — full opacity |
| **Pencil** | Slightly textured line with natural feel |
| **Marker** | Wide, semi-transparent strokes that layer |
| **Fine liner** | Razor-thin, crisp, full opacity |
| **Brush** | Medium width with pressure response |
| **Watercolor** | Organic pigment-blob stamps — velocity-sensitive |
| **Eraser** | Removes paint, reveals the paper background |

### Canvas Controls

| Control | How |
|---|---|
| **Undo** | `⌘Z` or the ↺ button in the top bar |
| **Redo** | `⌘⇧Z` or the ↻ button |
| **Zoom** | Scroll wheel (toward cursor) |
| **Pan** | Hold `Space` + drag |
| **Reset zoom** | Click the `100%` indicator in the top bar |
| **Export PNG** | Download button (top right) — composites paper background + drawing |

## Stack

- React 18 (UMD, no build step)
- HTML5 Canvas API
- Tailwind CSS (CDN)
- Babel Standalone (in-browser JSX)

## Running locally

```bash
python3 -m http.server 8080
```

Then open `http://localhost:8080/canvas-ui.html`.
