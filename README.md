# balmorehernandez.com

Hub page for Balmore Hernandez (**Master your body, mind and money.**), ES/EN, served by GitHub Pages
(user site `BalmoreHernandez/balmorehernandez.github.io`, custom domain `balmorehernandez.com`).

Every other Pages repo of the account without its own CNAME is served under this domain at `/<repo-name>/`:

| Path | Repo | Status |
|---|---|---|
| `/fitness/` | `BalmoreHernandez/fitness` | live |
| `/presupuesto/` | `BalmoreHernandez/presupuesto` | live |
| `/invoices/` | `BalmoreHernandez/invoices` | live |

## Editing
- `index.html` → `CONFIG.APPS.presupuesto.live = true` when `/presupuesto/` is published (card turns into an "Open the app" button).
  Also set `PRESUPUESTO_LIVE = true` in `404.html` so /budget, /finanzas… redirect to it.
- `CONFIG.SOCIAL`, `CONFIG.WHATSAPP`, `CONFIG.WA_TEXT`, texts in `I18N` (es/en).
- Styles in `style.css` (brand G8b: navy #0E1A2E, burgundy #A3263A, cream #F6F1E9, white cards, 22px corners, Montserrat/Inter self-hosted in `fonts/`).
- `404.html`: friendly not-found page that redirects old or mistyped paths (/app, /Fitness, /budget…).

All apps share the origin `balmorehernandez.com`: each app must use its own localStorage key and its own service-worker cache prefix (and only delete caches with that prefix).

## DNS (GoDaddy)
`@` A → 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153 · `@` AAAA → 2606:50c0:8000::153 … 8003::153 · `www` CNAME → balmorehernandez.github.io

## Change log
- 2026-10-07 — Added the Invoices card (`/invoices/`), its 404 redirects and the table row — Nico (Claude Cowork)
