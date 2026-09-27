# UK & France Travel Atlas

An interactive bilingual travel atlas for exploring places across Great Britain and France. Zoom in to reveal more destinations, hover over a place to illuminate its region, and open a compact guide to its highlights and nearby stops.

**Live demo:** https://shiqiaozhou.github.io/travel-atlas/

## Explore

- A softly illustrated, 2.5D-style map with rivers, terrain, coastlines, and administrative boundaries.
- Zoom-dependent detail: major destinations lead at overview scale; more places and labels appear as you zoom in.
- Each place has its own icon, an interactive highlighted area, and a bilingual mini-guide.
- Searchable-feeling exploration through hover, click-to-pin, nearby-place links, and keyboard-accessible markers.
- Chinese, English, and bilingual display, with responsive controls for smaller screens.

## Built with

Vanilla HTML, CSS, and JavaScript, with D3.js for the interactive map and TopoJSON for geographic shapes. The project is a single static `index.html` and does not require a build step.

## Run locally

Open `index.html` in a modern browser. An internet connection is used to load optional Google Fonts; system font fallbacks are included.

## Project notes

This is an AI-assisted creative-coding project. I shaped the map concept and interaction goals, then iterated on zoom-based detail, label spacing, regional highlighting, bilingual content, and mobile behavior with AI-assisted implementation.

## Credits

- Geographic boundaries and map shapes are based on Natural Earth data.
- D3.js v7.9.0 and TopoJSON v3.0.2; copyright notices are retained in the source file.
- Chinese and English typefaces are served by Google Fonts when available.
