# 🏝️ Living the Dream — Island Map Generator

A lightweight, high-performance web application to procedurally generate island terrain maps with ocean, organic sandy beaches, and grass layers. Shape the base layer of your island and **bake it directly into your `map.sav`**, or export it to **TomoDraft** (`.json`) for further pathing and building placement.

![HTML5 Canvas](https://img.shields.io/badge/Tech-Vanilla%20JS%20%2F%20HTML5%20Canvas-gold?style=flat-square)
![Deploy](https://img.shields.io/badge/Deploy-Cloudflare%20Pages%20%2F%20GitHub%20Pages-4A90C4?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)

---

## ✨ Features

### 💾 Direct `map.sav` Integration (NEW)
- **Import & Preview**: Load your existing game save (`map.sav`) directly into the browser to preview your current terrain, houses, and facilities on the canvas.
- **Bake to Save File**: Export your procedurally generated island directly back into your `map.sav`. Your buildings, Miis, and progression stay exactly as they are—only the terrain gets replaced.
- **Decor Cleanup**: Optional toggle to automatically strip out old decorations, paths, and user-generated content (UGC) from the save while preserving critical buildings.

### 🗺️ Procedural Island Generation
- **Seeded 2D Value Noise**: Creates natural, organic coastlines.
- **Multi-Island Support**: Generate 1 to 7 independent islands with customizable inter-island distance/spacing.
- **1% to 90% Water Ratio**: Precise slider control allowing maps from 99% land with a tiny 1% ocean fringe up to tiny archipelago islets.
- **Organic Beaches**: Toggle bigger beaches and adjust beach sectors (up to 3 beaches per island).

### 🖥️ Interactive Canvas & Tools
- **Live Viewport**: Smooth click & drag panning, mouse wheel zoom, pinch-to-zoom for mobile, and reset view controls.
- **Live Grid Coordinates Badge**: Displays real-time tile coordinates (`📍 X: --, Y: --`) on mouse movement.
- **Pixel Grid & Legend**: Toggleable grid overlay and dynamic legend for terrain and building markers.
- **TomoDraft Export**: One-click export to `.json` format compatible with TomoDraft for early planning.

---

## 🛠️ Project Structure

```text
island-generator/
├── index.html     # Complete web application (HTML, CSS, JS, Canvas & Save Parsing)
├── assets/        # App logo and favicon asset
│   └── favicon.png
└── README.md      # Project documentation
