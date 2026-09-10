# Seizure During Craniotomy

Static site hosted on GitHub Pages, covering intraoperative seizure
management during craniotomy, with an interactive crisis simulator.

## Project layout

```
conference/
├── index.html           # Seizure Management page — edit this directly
├── simulator.html        # Simulator tab — self-contained (own inline CSS/JS)
├── assets/
│   ├── style.css
│   ├── gaba-receptor.svg   # brand mark + favicon
│   ├── neurons-xenon.svg   # hero artwork
│   └── img/
├── CNAME                # custom domain
└── .nojekyll             # serve files as-is on GitHub Pages
```

There is no build step or generator — both pages are hand-edited plain HTML.
`index.html` uses the shared `assets/style.css`; `simulator.html` is a
self-contained single-file app (its own `<style>`/`<script>`), sharing only
the top nav tabs and site favicon. It is courtesy of Soowon Lee, MD, PhD
(Dept. of Anesthesiology & Pain Medicine, Seoul National University Bundang
Hospital) — credited on the page itself, don't remove that.

## Deploying to GitHub Pages

1. Push this folder to a GitHub repository.
2. Repo **Settings → Pages** → Source: *Deploy from a branch* → branch `main`,
   folder `/ (root)`.
3. The `CNAME` file points the site at its custom domain; add the matching DNS
   records at your DNS provider, then enable *Enforce HTTPS*.
