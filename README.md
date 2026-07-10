# InFlight — Prototype Suite

Interactive prototypes for a VC-native data platform: capture everything at the infrastructure layer, change no user workflows, and turn online/offline community into proprietary sourcing, formation, and nurturing loops.

## Contents

```
index.html                                  Landing hub (start here)
prototypes/
  inflight-core.html                        Core 5 screens: Radar, Graph, RFS, Intros, Flywheel
  inflight-deep-dive.html                   4 modules × 2 screens: VC-native CDP, Targeting, Nurturing, Ecosystem
  inflight-formation-readiness.html         10 unintuitive skills → formation decisions (interactive)
  inflight-expansion.html                   Modules 5–7: LP Console, Portfolio Telemetry, Graph Copilot
assets/
  vc-shadow-data-layer-architecture.svg     Block diagram of the shadow data layer
```

Static HTML/CSS/JS — no build step, no dependencies (Google Fonts via CDN).

## Run locally

```bash
npm start
# → http://localhost:8000
```

Or open `index.html` directly in a browser.

## Push to GitHub

```bash
cd inflight   # or your local clone path
git add -A && git commit -m "InFlight prototype suite"
gh repo create inflight --public --source=. --push
# or manually:
# git remote add origin git@github.com:<you>/inflight.git
# git branch -M main && git push -u origin main
```

## Host it

### GitHub Pages

1. Push to GitHub (see above)
2. Repo **Settings → Pages**
3. Source: deploy from `main` branch, `/` (root)
4. Site: `https://<you>.github.io/inflight/`

`.nojekyll` is included so GitHub Pages serves static files as-is.

### Vercel

```bash
npx vercel
```

Framework preset: **Other**. `vercel.json` is included — zero build step needed.

Or connect the GitHub repo in the [Vercel dashboard](https://vercel.com/new) for automatic deploys on push.

## Keyboard shortcuts

- Core prototype: keys `1–5` switch screens
- All screens are responsive down to mobile widths
