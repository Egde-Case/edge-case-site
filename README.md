# Edge Case site

Static, single file. Deploy on GitHub Pages:

1. Put `index.html` and `.nojekyll` at the root of the repo (or in `/docs`).
2. Settings → Pages → Source: Deploy from a branch → pick the branch and folder.
3. Add a `CNAME` file containing only your domain (e.g. `edgecase.example`) and point the domain's DNS at GitHub Pages (A records 185.199.108.153 / .109 / .110 / .111, plus a CNAME for `www` → `<user>.github.io`).

Fonts load from Google Fonts (Barlow, Caveat). No build step, no dependencies.
