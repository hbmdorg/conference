# Seizure During Craniotomy

Single-page static site hosted on GitHub Pages, covering intraoperative
seizure management during craniotomy.

## Project layout

```
conference/
├── index.html          # the whole site — edit this directly
├── assets/
│   ├── style.css
│   ├── gaba-receptor.svg   # brand mark + favicon
│   ├── neurons-xenon.svg   # hero artwork
│   └── img/
├── CNAME                # custom domain
└── .nojekyll             # serve files as-is on GitHub Pages
```

There is no build step or generator — `index.html` is hand-edited plain HTML.

## Deploying to GitHub Pages

1. Push this folder to a GitHub repository.
2. Repo **Settings → Pages** → Source: *Deploy from a branch* → branch `main`,
   folder `/ (root)`.
3. The `CNAME` file points the site at its custom domain; add the matching DNS
   records at your DNS provider, then enable *Enforce HTTPS*.
