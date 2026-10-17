# RouteIQ — Intelligent Logistics Lab

Responsive interactive logistics routing prototype. Static files only; no backend/build step required.

## Features
- 25-node synthetic road graph, rendered as interactive SVG.
- Configure start, destination, and ordered delivery stops.
- Close/reopen roads and recalculate.
- BFS and Dijkstra implementations with explored-node metrics.
- Route distance, illustrative time/cost estimates, and algorithm comparison.
- Research, methodology, architecture, limitations, and future-work sections.

## Run locally
Open `index.html` in a modern browser. No install required.

## Publish on GitHub Pages
1. Create a repository on GitHub.
2. Upload `index.html`, `style.css`, `app.js`, and `README.md` to the repository root.
3. Open **Settings → Pages**.
4. Choose **Deploy from a branch**, select `main` and `/ (root)`, then save.
5. Open the published URL shown by GitHub Pages.

## Important assumptions
This is an educational simulation, not a live dispatch tool. The network is synthetic; it does not use real roads, GPS, traffic, weather, or fleet data. Each edge costs one unit. Estimated time is route edge count × 1 minute; estimated cost is route edge count × $2.50. These are illustrative assumptions, not measured results. Delivery stops are visited in the order entered, not globally optimized. BFS finds a fewest-edge path in an unweighted graph; Dijkstra finds a minimum-cost path for non-negative edge weights.

Review the original research before claiming any specific statistic or conclusion comes directly from it.
