# World Population 3D Globe

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![WebGL](https://img.shields.io/badge/Render-WebGL-brightgreen.svg)](#)
[![Zero Dependency](https://img.shields.io/badge/Build-Zero%20Dependency-orange.svg)](#)

An interactive, high-performance 3D visualization of world country populations mapped across a spherical Earth model. Each country's boundary is extruded into a 3D polygon whose height and color dynamically represent its population size.

---

## Highlights

- **3D Polygonal Extrusion**: Accurate radial extrusion mapping population density to altitude using a non-linear (square-root) scale to preserve visibility for both high-population and small nations.
- **Dynamic Choropleth Palette**: Smooth multi-stop gradient ranging from deep navy (`<10M`), cyan (`~50M`), emerald (`~100M`), amber (`~500M`), to coral/red (`1B+`).
- **Interactive Tooltips**: Hover over any country to reveal country name, formatted population, and UN geographic region.
- **Atmospheric Glow & Lighting**: Subtle blue atmosphere curvature and dark tech aesthetic with glassmorphism UI overlays.
- **Zero-Build & Offline Ready**: Standalone vanilla HTML/JS bundled with local `countries-data.js` (177 countries) and offline `globe.gl.min.js` (with automatic fallback to CDN).

---

## Controls

| Action | Control |
|---|---|
| **Rotate Globe** | Left-click + Drag |
| **Pan Camera** | Right-click + Drag |
| **Zoom In / Out** | Mouse Wheel / Touch Pinch |
| **Inspect Country** | Hover cursor over landmass |
| **Toggle Auto-Rotate** | Click `Auto-Rotate` button in top right |
| **Reset View** | Click `Reset View` button |

---

## Quick Start

### 1. Direct Browser Launch
Simply open `index.html` directly (no web server required):
```bash
open index.html
```

### 2. Local HTTP Server
Alternatively, serve via any static file server:
```bash
# Python 3
python3 -m http.server 8000

# Node.js (npx)
npx serve .
```
Then navigate to `http://localhost:8000`.

---

## Data Source & Attribution

- **Cartography & Population Data**: Derived from [Natural Earth](https://www.naturalearthdata.com/) Admin 0 Country boundaries (`ne_110m_admin_0_countries.geojson`), featuring 177 sovereign territories and population estimates.
- **Core 3D Engine**: Powered by [Three.js](https://threejs.org/) and [Globe.gl](https://globe.gl/).

---

## License

This project is licensed under the [MIT License](LICENSE) - see the LICENSE file for details.
