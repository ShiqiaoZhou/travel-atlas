# UK & France Travel Atlas

An interactive bilingual travel atlas for exploring places across Great Britain and France. Zoom in to reveal more destinations, hover over a place to illuminate its region, and open a compact guide to its highlights and nearby stops.

**Live demo:** https://shiqiaozhou.github.io/travel-atlas/

## Explore

- A softly illustrated, 2.5D-style map with rivers, terrain, coastlines, and administrative boundaries.
- Zoom-dependent detail: major destinations lead at overview scale; more places and labels appear as you zoom in. City markers and names grow subtly with zoom, up to 12%.
- Each place has its own icon, an interactive highlighted area, and a bilingual mini-guide.
- Destination cards include one cover photo and one photo for each featured attraction. Photos load as needed and link to their Wikimedia Commons source with available author and license details.
- Searchable-feeling exploration through hover, click-to-pin, nearby-place links, and keyboard-accessible markers.
- Chinese, English, and bilingual display, with responsive controls for smaller screens.

## New UK city guides

The latest update adds six destinations, bringing the UK map to 35 places:

- **Bristol** — Clifton Suspension Bridge, the Harbourside, and SS Great Britain.
- **Durham** — the cathedral, castle, and River Wear loop.
- **Norwich** — the cathedral, Norman castle, and Elm Hill.
- **Chester** — the Roman walls, Tudor Rows, and cathedral.
- **Canterbury** — the cathedral, St Augustine’s Abbey, and River Stour.
- **Salisbury** — its soaring cathedral, Magna Carta, and Old Sarum.

## Built with

Vanilla HTML, CSS, and JavaScript, with D3.js for the interactive map and TopoJSON for geographic shapes. The project is a single static `index.html` and does not require a build step.

## Run locally

Run a local static server from the project folder, then open `http://127.0.0.1:8767/`:

```sh
python3 -m http.server 8767
```

No build step is required. An internet connection is used for Google Fonts and on-demand destination photos; system font fallbacks are included.

## Project notes

This is an AI-assisted creative-coding project. I shaped the map concept and interaction goals, then iterated on zoom-based detail, label spacing, regional highlighting, bilingual content, and mobile behavior with AI-assisted implementation.

## Credits

- Geographic boundaries and map shapes are based on Natural Earth data.
- D3.js v7.9.0 and TopoJSON v3.0.2; copyright notices are retained in the source file.
- Chinese and English typefaces are served by Google Fonts when available.
- Destination and attraction photographs are fetched from Wikimedia Commons with source, author, and available license details shown in each card.
