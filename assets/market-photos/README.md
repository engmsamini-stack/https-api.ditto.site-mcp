# Market page photos

Curated, free-to-use stock photo candidates for the 13 market/industry pages
(Commercial, Data Centers, Mission Critical, Education, Healthcare, Life
Sciences, Government & Federal, Municipal, Industrial & Manufacturing,
Semiconductors, Renewables & Solar, EV Charging Infrastructure, Mixed-Use &
Multi-Family Residential).

See [`markets.json`](./markets.json) for the full machine-readable list —
one entry per market with 2–3 ranked photo picks, source page, photographer
credit, description, and suggested alt text.

## Sources & licensing

All picks come from **Unsplash**, **Pexels**, or **Pixabay**. Each of these
offers a free license that permits commercial/website use with no royalty
and no attribution legally required (attribution is still a nice courtesy).
Every `sourceUrl` in `markets.json` is a real page found via live search —
none are fabricated.

## Why there's no image file / direct CDN URL yet

This was curated from an environment where outbound network access to
unsplash.com, pexels.com, and pixabay.com is blocked, so the direct
`images.unsplash.com/...`, `images.pexels.com/...`, or `cdn.pixabay.com/...`
URLs could not be fetched or verified, and no binary image files could be
downloaded into this directory.

**To finish wiring a photo into the site:**
1. Open the pick's `sourceUrl`.
2. Click "Download" (Unsplash/Pexels/Pixabay all offer free downloads —
   pick a size appropriate for web use, e.g. ~1600–2400px wide).
3. Either:
   - Save the file into this directory (e.g. `commercial-01.jpg`) and
     reference it locally, or
   - Copy the CDN URL Unsplash/Pexels/Pixabay serve and hotlink it directly
     (all three permit hotlinking).
4. Use the `altText` field from `markets.json` for the `<img alt>`.

## Known gaps (flagged during research, not silently guessed around)

- **Mission Critical** — no credible free photo of an emergency operations
  center / control room was found; picks are hospital exteriors instead.
- **Semiconductors** — no genuine free photo of a cleanroom "bunny suit"
  technician on a fab floor was found (the term collides with unrelated
  stock content). Picks are the closest honest matches (wafer lab,
  cleanroom equipment); consider a paid library (Getty/iStock) for this
  page specifically if a fab-floor/bunny-suit shot is important.
- A few photographer credits are marked "verify on page" where the search
  index surfaced a curator/tag rather than the confirmed photographer.
