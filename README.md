# US Transplant Center Volumes

Interactive dashboard of all active US abdominal transplant programs: kidney and liver volumes split by donor type for 2021-2025 plus 2026 year-to-date, growth badges, 2026 pace, and click-to-expand five-year trend panels per center. Living-donor kidney and liver shares, plus leader cards for the fastest-growing programs. Works on phone and desktop.

`index.html` is fully self-contained: no build step, no dependencies. Data is embedded in the page (OPTN National Data, hrsa.unos.org) and refreshed monthly; the data date is shown at the top of the page.

## How to publish (GitHub Pages)

1. Create a new **public** repository on GitHub (e.g., `transplant-volumes`).
2. Upload `index.html` (and this README) to the repo.
3. In the repo: **Settings -> Pages -> Build and deployment -> Source: Deploy from a branch**, pick `main` / `root`, Save.
4. Open it at `https://<your-username>.github.io/transplant-volumes/`.

## Monthly updates

A scheduled task refreshes the app data on the 1st of each month and rewrites this folder's `index.html`. GitHub does not update itself: after a refresh, re-upload `index.html` to the repo (drag-and-drop on github.com works) or `git commit && git push`, and the same link serves the new data.
