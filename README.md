# Fund OS — Signal Desk Prototype Suite

Interactive prototypes for a product + data leadership thesis at an events-driven early-stage VC: capture everything at the infrastructure layer, change no user workflows, and turn online/offline community into proprietary sourcing, formation, and nurturing loops.

## Contents

```
index.html                                  Landing hub (start here)
prototypes/
  fund-os-prototype.html                    Core 5 screens: Radar, Graph, RFS, Intros, Flywheel
  fund-os-4x2-prototype.html                4 modules x 2 screens: VC-native CDP, Targeting, Nurturing, Ecosystem
  formation-readiness-profiler.html         10 unintuitive skills -> formation decisions (interactive)
  fund-os-expansion.html                    Modules 5-7: LP Console, Portfolio Telemetry, Graph Copilot
assets/
  vc-shadow-data-layer-architecture.svg     Block diagram of the shadow data layer
```

Everything is static HTML/CSS/JS with zero build step and zero dependencies (Google Fonts loaded via CDN; degrades gracefully offline).

## Run locally (Cursor)

1. Open this folder in Cursor (`File > Open Folder`)
2. Either:
   - Install the **Live Server** extension, right-click `index.html` → *Open with Live Server*, or
   - Run from the integrated terminal: `python3 -m http.server 8000` then visit `http://localhost:8000`
3. You can also just double-click `index.html` — no server strictly required.

## Push to GitHub

```bash
cd fund-os-suite
git init && git add -A && git commit -m "Fund OS prototype suite"
gh repo create fund-os-suite --private --source=. --push
# or manually:
# git remote add origin git@github.com:<you>/fund-os-suite.git
# git branch -M main && git push -u origin main
```

## Host it

- **GitHub Pages:** repo Settings → Pages → deploy from `main` / root. Site appears at `https://<you>.github.io/fund-os-suite/`
- **Vercel:** `npx vercel` from the folder (framework preset: Other). Zero config needed.

## Keyboard shortcuts

- Core prototype: keys `1–5` switch screens
- All screens are responsive down to mobile widths
