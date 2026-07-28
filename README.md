# 🏝️ Living the Dream — Island Map Generator

A lightweight, high-performance web application to procedurally generate island terrain maps with ocean, organic sandy beaches, and grass layers. Designed to create base terrain maps and export them directly to **TomoDraft** (`.json`) for further pathing and building placement.

![HTML5 Canvas](https://img.shields.io/badge/Tech-Vanilla%20JS%20%2F%20HTML5%20Canvas-gold?style=flat-square)
![Deploy](https://img.shields.io/badge/Deploy-Cloudflare%20Pages%20%2F%20GitHub%20Pages-4A90C4?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)

---

## ✨ Features

- **Procedural Island Generation**: Seeded 2D Value Noise algorithms create natural, organic coastlines.
- **1% to 90% Water Ratio**: Precise slider control allowing maps from 99% land with a tiny 1% ocean fringe up to tiny archipelago islets.
- **Multi-Island Support**: Generate 1 to 7 independent islands with customizable inter-island distance/spacing.
- **Organic Beaches & Custom Beach Count**: Toggle bigger beaches and adjust beach sectors per island.
- **Interactive Viewport**: Smooth click & drag panning, mouse wheel zoom, pinch-to-zoom for mobile, and reset view controls.
- **Live Grid Coordinates Badge**: Displays real-time tile coordinates (`📍 X: --, Y: --`) on mouse movement.
- **Pixel Grid Overlay**: Toggleable grid overlay for precise mapping preview.
- **TomoDraft Export**: One-click export to `.json` format compatible with TomoDraft.
- **Zero External Dependencies**: Standalone single-page web app using pure HTML, CSS, and Vanilla JavaScript.

---

## 🛠️ Project Structure

```text
island-generator/
├── index.html     # Complete web application (HTML, CSS, JS & Canvas rendering)
├── favicon.png    # App logo and favicon asset
└── README.md      # Project documentation
```

---

## 🚀 Deployment Instructions

### 🌐 Cloudflare Pages (Recommended)

#### Option 1: Direct Upload (Drag & Drop)
1. Log in to the [Cloudflare Dashboard](https://dash.cloudflare.com/) and navigate to **Workers & Pages**.
2. Click **Create Application** → **Pages** → **Upload assets**.
3. Name your project (e.g., `island-generator`).
4. Drag and drop the repository folder or upload `index.html` and `favicon.png`.
5. Click **Save and Deploy**.

#### Option 2: Connect to GitHub Repository
1. Push this repository to GitHub.
2. In Cloudflare Pages, select **Connect to Git** and pick your repository.
3. Set the following build settings:
   - **Framework preset**: None
   - **Build command**: *(leave empty)*
   - **Build output directory**: `/` (or leave as root)
4. Click **Save and Deploy**.

#### Option 3: Wrangler CLI
```bash
npx wrangler pages deploy . --project-name=island-generator
```

---

## 💻 Local Development

No build step or server setup is required!

1. Clone or download the repository.
2. Open `index.html` directly in any modern web browser.
3. *(Optional)* Serve locally using VS Code Live Server or Python:
   ```bash
   python -m http.server 8000
   ```

---

## 📄 License

Distributed under the MIT License. Feel free to modify and use in your own projects.
