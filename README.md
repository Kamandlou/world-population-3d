# World Population 3D Globe

A lightweight, zero-dependency 3D interactive Earth visualization displaying the population of all world countries using extruded 3D polygons and dynamic color gradients.

## Features
- **3D Polygon Extrusion**: Country heights scaled by square-root of population for clear visual contrast.
- **Color Mapping**: Dynamic multi-stop gradient (blue → cyan → green → amber → red) mapped to population scale.
- **Interactive Tooltips**: Hover over any country to see its name, formatted population, and UN region.
- **Camera Controls**: Orbit, pan, zoom, smooth auto-rotation toggle, and reset view.
- **Offline Ready**: Bundled with local `countries-data.js` (177 countries) and `globe.gl.min.js` with CDN fallbacks.

## Quick Start

Open directly in your browser:
```bash
open index.html
```

Or run via any local HTTP server:
```bash
python3 -m http.server 8000
```
Then visit `http://localhost:8000`.
