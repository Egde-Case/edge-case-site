# Edge Case site

Static, two pages, no build step.

- `index.html` is the desktop site. On a touch device narrower than 760px it redirects to `m.html`.
- `m.html` is the mobile site, laid out for one column and a thumb. Its footer has a "Desktop site" link, which pins the desktop version for that browser session.
- `.nojekyll` keeps GitHub Pages from running Jekyll.

Deploy on GitHub Pages:

1. Put `index.html`, `m.html` and `.nojekyll` at the root of the repo (or in `/docs`).
2. Settings → Pages → Source: Deploy from a branch → pick the branch and folder.
3. Add a `CNAME` file containing only your domain and point DNS at GitHub Pages (A records 185.199.108.153 / .109 / .110 / .111, plus a CNAME for `www` → `<user>.github.io`).

Fonts load from Google Fonts (Barlow, Caveat).
