# SIAR Digital — Service Packages

Sales collateral for SIAR Digital's three service lines across five markets
(Pakistan, GCC, United States, Canada, Mexico).

## Files

| File | Audience | Purpose |
|---|---|---|
| `strategy.md` | **Internal** | Single source of truth: market/competitor analysis (with sources), full pricing tables, financial model, capacity model, commercial terms, SOWs, objection handling. |
| `index.html` | **Client-facing** | Branded, self-contained page with a market switcher. Shows SOW · Price · Timeline per tier, the flagship bundle, payment terms, and the launch-date protection model. Matches the house style of the main blog. |

## How to update prices

Prices live in **two** places — keep them in sync:

1. **`strategy.md` §4 Price book** — the authoritative tables.
2. **`index.html`** — the `MARKETS` JavaScript object near the bottom of the file
   (one entry per market: `build`, `ref`, `ops`, `seo`, `bundle` per tier).

Tier **scope** (SOW bullets, timelines) is defined once in the `TIERS` array in
`index.html` and shared across every market — edit it there to change scope everywhere.

FX anchors used: 1 USD ≈ 278 PKR · 3.67 AED · 3.75 SAR · 1.37 CAD · 18 MXN.
Review the PKR card and local-currency reference lines quarterly as FX moves.

## Notes

- The `[REPLACE-WITH-OG-IMAGE-1200x630].jpg` placeholder in `index.html` should be
  swapped for a real social-share image before publishing.
- AEO/GEO is bundled into the displayed SEO figure (a ~40% premium layer) and is also
  sold standalone — see `strategy.md` §4.6.
