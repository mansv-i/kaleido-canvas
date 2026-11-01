# Symmetry · Kaleidoscope Drawing Studio

A zero-dependency, self-contained interactive kaleidoscope and mandala drawing studio built with vanilla HTML5 Canvas and CSS. 

Draw with a mouse, touch, or pen to mirror strokes in real time across 2 to 24 radial axes, or let autonomous generative mode create evolving patterns.

---

## Features

* **Multi-Axis Radial Symmetry:** Real-time canvas stroke mirroring from 2-fold up to 24-fold symmetry.
* **Bilateral Mirroring:** Optional secondary axis reflection for true mandala geometry.
* **Dream Mode:** Autonomous generative drawing engine powered by parametric trigonometric paths (`sin`/`cos` Lissajous-style curves).
* **Brush Modes & Customization:**
  * **Rainbow:** Continuous HSL color cycling based on stroke distance.
  * **Palettes:** 5 curated color schemes with linear RGB interpolation.
  * **Solid:** Native HTML5 color-picker support.
  * **Effects:** Adjustable brush diameter (1–24 px), additive neon glow (`lighter` compositing + shadow blur), and fading motion trails.
* **Pointer & Device Support:** Native Pointer Events API (`pointerdown`, `pointermove`, `pointerup`) with coalesced event handling for smooth curves across desktop, tablet, and mobile.
* **Canvas State Management:** In-memory canvas snapshots supporting 15-step undo history (`Z` / `Ctrl+Z`) and canvas clearing (`C`).
* **High-Res PNG Export:** Merges current path buffer over a gradient background canvas for 1-click downloads.
* **Offline & Self-Contained:** Embedded WOFF2 typefaces (Syne & Space Grotesk) and zero runtime npm dependencies—runs directly in any modern browser via a single file.

---

## Keyboard Shortcuts

| Key | Action |
| :--- | :--- |
| **`Z`** / **`Ctrl + Z`** | Undo previous stroke |
| **`C`** | Clear canvas |
| **`D`** | Toggle Dream Mode (autonomous drawing) |
| **`H`** | Toggle controls panel visibility |
| **`[`** / **`]`** | Decrease / Increase symmetry folds |
| **`-`** / **`=`** | Decrease / Increase brush diameter |

---

## Getting Started

Because this project is built as a single, self-contained HTML file:

1. Clone or download the repository:
   ```bash
   git clone [https://github.com/](https://github.com/)<your-username>/symmetry.git
