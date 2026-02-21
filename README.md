# SVCA Group Website

**SVCA Group** is a holding company operating at the intersection of deep technical infrastructure and high-end brand strategy.

This repository houses the single-page static landing site for the firm. There are no frameworks, no external libraries, and no bloat. It is a zero-dependency HTML/CSS architecture built to execute a single visual metaphor with absolute mathematical precision.

## The Design Philosophy

The site is built to visually represent the bridging of our two core disciplines:

1. **Systems & Intelligence:** Fractional CTO, Architecture, and AI Consulting.
2. **Stories & Strategy:** Creative Production, Brand Identity, and Narrative Strategy.

To reflect this, the site is designed as a living architectural blueprint. It uses strict geometric constraints to ground highly editorial typography, proving that creativity and structural engineering can coexist seamlessly.

## Technical Intentionality & Execution

Every pixel on the screen is placed using strict absolute mathematics.

### 1. The Blueprint Grid (Sub-Pixel Rendering)

Standard web grids often float imperfectly depending on viewport size. To guarantee that the grid serves as an absolute source of truth, the background origin is mapped to the exact mathematical center of the screen `calc(50vw - 0.5px) calc(50vh - 0.5px)`. This offset forces the mathematical `0px` starting point of the screen to align perfectly with the absolute center of the pixel grid, eliminating blurry sub-pixel rendering.

### 2. Absolute Mathematical Lines

Standard CSS borders (`border: 1px solid`) render *inside* their bounding boxes, which causes a 1px mismatch when overlaid on a background grid. To achieve undeniable perfection, CSS borders were abandoned entirely.

The structural drafting lines are built using `1px` absolute `div` elements with a `transform: translate(-50%)` applied. This mathematically slices the 1px line exactly in half over the coordinate, resulting in an impossible-to-miss overlap with the underlying grid.

### 3. Typographic Tension

The typography reflects the dual nature of the firm:

* **SVCA:** Set in **Cormorant Garamond** (Editorial / Creative / Humanistic). Because serif fonts have complex ascenders and descenders, an optical baseline shift (`padding-top: calc(var(--minor) * 0.3)`) is hard-coded to pull the text down so it locks perfectly onto the horizontal crosshairs.
* **GROUP:** Set in **Inter** (Structural / Modern / Tech). The sub-brand is locked inside a strictly defined minor-grid container, mathematically preventing it from bleeding outside its designated row.

### 4. The Reveal (Animation)

The load sequence is highly intentional. The core framing and typography fade in first—presenting a minimal, confident brand identity. After a 1.5-second delay, the foundational grid fades in behind it. This sequential reveal demonstrates to the viewer that the minimal design isn't floating arbitrarily; it is anchored to a strict, intentional coordinate system.

## Deployment

This site is a single `index.html` file deployed via GitHub Actions.

To run locally:

1. Clone the repository.
2. Open `index.html` in any modern web browser.

---
*Architected for SVCA Group.*
