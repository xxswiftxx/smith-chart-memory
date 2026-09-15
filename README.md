# The Smith-Chart-for-Memory site

Three self-contained pages about a fun experiment: using a 1939 RF **Smith chart** as a lens for AI memory
retrieval. Everything runs in the browser — the only external dependency is Google Fonts.

## Pages
- **index.html** — the story ("A 1939 Radio Chart, Pointed at Memory"): the write-up, with an interactive
  Smith disk and a "re-ask the question" locus animation. The one to share.
- **essay.html** — "The Smith Chart Is Not a Ranker": the design-thesis version, with a worked walk-through.
- **explorer.html** — the full interactive Γ-Locus Explorer (all five facets: locus, matching networks,
  cluster matching, aging sweep, active reconciliation, plus the Retrieval TDR view).

They cross-link to each other with relative paths, so the folder works as one site.

## Deploy on GitHub Pages (drag-and-drop-ish)
1. Make a new GitHub repo (e.g. `smith-memory`).
2. Add these files to it (`index.html`, `essay.html`, `explorer.html`, `README.md`) at the repo root.
3. Repo **Settings → Pages → Build and deployment → Source: Deploy from a branch → main / (root) → Save**.
4. Wait ~1 minute. Your site is live at `https://<your-username>.github.io/smith-memory/`.

`index.html` is served automatically as the home page.

## Or: Netlify (no repo needed)
Go to app.netlify.com/drop and drag this whole `site` folder onto the page. Instant public URL.

## Putting it on LinkedIn
LinkedIn can't embed live HTML, so:
- Post the **link** to your Pages/Netlify URL (people click through to the live interactive), **and/or**
- Post a short **screen-recording / GIF** of the "re-ask the question" animation for in-feed engagement.

## Notes
- Fully static — no server, no build step, no tracking.
- Needs internet only to fetch the fonts; it still renders with fallback fonts offline.
- Light/dark aware (follows the viewer's system theme).
