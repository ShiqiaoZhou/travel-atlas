# UK & France Travel Atlas

An interactive bilingual travel atlas for exploring places across Great Britain and France. Zoom in to reveal more destinations, hover over a place to illuminate its region, and open a compact guide to its highlights and nearby stops.

**Live demo:** https://shiqiaozhou.github.io/travel-atlas/

## Explore

- A softly illustrated, 2.5D-style map with rivers, terrain, coastlines, and administrative boundaries.
- Zoom-dependent detail: major destinations lead at overview scale; more places and labels appear as you zoom in. City markers and names grow subtly with zoom, up to 12%.
- Each place has its own icon, an interactive highlighted area, and a bilingual mini-guide.
- Destination cards include one cover photo and one photo for each featured attraction. Photos load as needed and link to their Wikimedia Commons source with available author and license details.
- Searchable-feeling exploration through hover, click-to-pin, nearby-place links, and keyboard-accessible markers.
- Chinese, English, and bilingual display, with touch-friendly controls and an expandable place guide on phones. Attraction photos use readable full-width rows in the mobile guide.

## 64 new destinations

The latest update adds 32 places in each country, bringing the atlas to **67 places in the UK and 60 in France**. Most appear as you zoom in, so the overview stays uncluttered.

- **England** — Peak District, Yorkshire Dales, Whitby, Castle Howard, Newcastle, Alnwick, Lindisfarne, Lincoln, Winchester, Portsmouth, New Forest, Isle of Wight, Rye, Warwick, Blenheim Palace, St Michael's Mount, Tintagel, Eden Project, Wells, and Ironbridge Gorge.
- **Scotland** — Glen Coe, Oban, Stirling, St Andrews, Glenfinnan, the Cairngorms, Orkney, and Eilean Donan.
- **Wales & Northern Ireland** — Pembrokeshire Coast, Brecon Beacons, Caernarfon, and Derry.
- **Northern France** — Fontainebleau, Chantilly, Honfleur, Rouen, Amiens, Chartres, Épernay, Nancy, and Haut-Kœnigsbourg.
- **Western France** — Nantes, the Pink Granite Coast, Quimper, La Rochelle, Cognac, Dune du Pilat, and Sarlat.
- **Central France & Burgundy** — Dijon, Beaune, Vézelay, Puy de Dôme, Le Puy-en-Velay, and Rocamadour.
- **Southern France** — Albi, Millau Viaduct, Montpellier, Collioure, Arles, the Camargue, Gordes, Aix-en-Provence, Cannes, and Saint-Tropez.

The map also now opens on iPhone and Safari: the background grid is limited to Western Europe, which fixes a freeze in WebKit.

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
