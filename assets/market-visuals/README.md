# Market page visuals

Thirteen original SVG illustrations, one per market page, designed as a
matched set — no stock photos, no licensing, no network dependency.

## Concept

Each sector is drawn as an engineering **drawing sheet**: a navy blueprint
background with a fine grid, corner crop marks, a north-arrow / sheet
furniture in the corner (drafting-sheet conventions), and a large
amber/cyan duotone line-art icon depicting the sector, framed by a title
block with a sheet number (A-01 through A-13). The motif ties directly to
the firm's own discipline — architecture, MEP, civil, structural design —
so the icons read as the firm's own drawings rather than generic clip art.

See [`manifest.json`](./manifest.json) for the full list (slug, filename,
title, alt text) and shared style tokens.

| # | File | Market |
|---|------|--------|
| A-01 | `commercial.svg` | Commercial |
| A-02 | `data-centers.svg` | Data Centers |
| A-03 | `mission-critical.svg` | Mission Critical |
| A-04 | `education.svg` | Education (K–12 & Higher Ed) |
| A-05 | `healthcare.svg` | Healthcare |
| A-06 | `life-sciences.svg` | Life Sciences |
| A-07 | `government-federal.svg` | Government & Federal |
| A-08 | `municipal.svg` | Municipal |
| A-09 | `industrial-manufacturing.svg` | Industrial & Manufacturing |
| A-10 | `semiconductors.svg` | Semiconductors |
| A-11 | `renewables-solar.svg` | Renewables & Solar |
| A-12 | `ev-charging.svg` | EV Charging Infrastructure |
| A-13 | `mixed-use-multifamily.svg` | Mixed-Use & Multi-Family Residential |

## Using them

Each file is a self-contained `.svg` (viewBox `0 0 480 360`, 4:3), safe to
use directly as an `<img src="...">`, a CSS `background-image`, or inlined.
No external fonts or assets are referenced (text uses the system monospace
stack), so they render correctly wherever they're dropped, including as a
plain `<img>` where external stylesheets don't apply. Each has a
`<title>`/`aria-label` for accessibility — reuse the `altText` from
`manifest.json` if wrapping in an `<img alt="...">`.

They commit to one fixed dark palette (not light/dark-adaptive) since
they're meant to be used as photographic-style hero/card art, the same way
the stock photos they replace would be.

## Why SVG instead of the photo manifest from `../market-photos/`

The earlier `market-photos/` manifest curated real free stock photo
candidates, but this sandbox's network policy blocks fetching from
unsplash.com/pexels.com/pixabay.com, so no actual image files could be
downloaded — only source links. These SVGs need no download step, no
license review, and no attribution, and stay perfectly on-brand. Both
folders are kept; use whichever fits the site's final direction (or swap
per-market as needed).
