# CURLABS — public site

The front door of Cur's lab. Static, zero dependencies, dark space theme.

## Structure

```
index.html              Landing page (hero, featured sim, projects, house, about)
styles.css              Theme (dark space, responsive)
solar-system/index.html Solar System Sim — single-file Three.js (three.js 0.160.0 via jsdelivr CDN)
```

## Deploy

Cloudflare Pages — **no build step** (output directory: repo root). Custom domain: `curlabs.net`. SSL auto-provisions.

**Updating:** push to `main` → Pages auto-rebuilds and deploys. That's the whole workflow.

## Rules

- **No dead links on day one.** A card gets a link only when the URL is real. Otherwise it says "in the lab."
- Site is public content only — no secrets, no internal data, no operational detail.
- Project cards: `index.html` → `.grid` → one `<article class="card">` each.

## History

- 2026-08-14: scaffolded by Ledger (bookkeeper) — v1 outline approved by Cur; SPP/Playerbots link verified (github.com/cmangos/playerbots, upstream main).
