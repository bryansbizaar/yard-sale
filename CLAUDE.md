# Claude Context — Yard Sale Shop

## Project Overview
A single-page static HTML shop for listing yard sale / secondhand items for sale. No framework, no build step — just HTML, inline CSS, and real product photos.

## Project Goals
- Display items for sale with photos, names, descriptions, and prices
- "Make an offer" section for items without fixed prices
- Rustic/handmade visual style borrowed from sister projects (react-tunes, queen-bee)
- Single-page: all nav links anchor to sections on the same page

## File Structure
```
yard-sale/
├── index.html                # Main HTML file (all styles inline)
├── CLAUDE.md                 # This file
└── pics/
    ├── for-sale/             # Items with fixed prices
    │   ├── kitchen-hutch.jpeg
    │   ├── loft-table.JPG
    │   ├── story-stools.jpeg
    │   ├── water-table-open.jpeg
    │   ├── water-table-closed.jpeg
    │   ├── water-stands.jpeg
    │   ├── ladybug-swing.jpeg
    │   ├── small-hutch.jpeg
    │   ├── kitchen.jpeg
    │   ├── wooden-truck-open.jpeg
    │   └── IMG_*.jpeg        # Additional photos
    └── make-an-offer/        # Items without fixed prices
        ├── barn.jpeg
        ├── wood-blocks.jpeg
        ├── wooden-train.jpeg
        ├── wooden-truck.jpeg
        ├── drum.jpeg
        ├── doll.jpeg
        ├── crowns.jpeg
        ├── assorted-wooden-toys.jpeg
        ├── assorted-art-supplies.jpeg
        ├── percussion-instruments.jpeg
        ├── sandbox-toys.jpeg
        ├── sandbox-truck.jpeg
        ├── wooden-bowling-pins.jpeg
        ├── wooden-kitchen-toys.jpeg
        ├── wooden-ladder-ramp.jpeg
        ├── wooden-trailer.jpeg
        ├── wooden-animals-assorted.jpeg
        ├── wooden-clips.jpeg
        ├── wooden-coathooks.jpeg
        ├── wooden-platter.jpeg
        ├── ribbons.jpeg
        ├── painting-jars.jpeg
        ├── picnic-set.jpeg
        ├── kids-iron.jpeg
        └── IMG_*.jpeg        # Additional photos
```

## Design System

### Colors (from react-tunes + queen-bee)
- Body background: `rgb(231, 227, 215)` — warm greige
- Header gradient: `linear-gradient(135deg, #fee389 0%, #fad7d7 100%)`
- Nav bar: `rgb(247, 226, 181)` — warm golden yellow
- Card background: `rgb(253, 251, 245)` — off-white cream
- Title color: `#996f05`
- Price color: `#b8860b`
- Nav link color: `#7a5800`

### Fonts
- Headlines/title: Georgia serif
- UI text (nav, labels, prices, desc): `Economica` (Google Font, loaded via CDN)

### Text Shadows
- Shop title: `0.2rem 0.2rem 0.2rem rgba(0,0,0,0.25)`
- Nav links: `0.08rem 0.08rem 0.08rem rgba(0,0,0,0.15)`

## Key Conventions
- **All styles are inline** in the `<style>` block — no external CSS files
- **Image paths** reference `pics/for-sale/filename.jpeg` or `pics/make-an-offer/filename.jpeg`
- **No cart/buy buttons** — this is a display-only listing page
- **Single-page** — nav anchors use `#section-id` format
- **Responsive grid** using CSS `auto-fill` with `minmax(210px, 1fr)`

## Current Status
- Wireframe complete with placeholder cards and styled layout
- Real product photos available in `pics/` — ready to be wired into cards
- Next: replace placeholder cards with actual items and photos

## When Working With AI Assistants
- Reference `pics/for-sale/` for priced items and `pics/make-an-offer/` for unlisted items
- Keep everything in a single HTML file unless explicitly asked to split it out
- Preserve the rustic/handmade aesthetic — avoid modern flat/minimal redesigns
- Image paths in HTML should be relative: `pics/for-sale/filename.jpeg`
