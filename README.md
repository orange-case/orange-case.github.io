# orange-case.github.io

Static website for **The Orange Case**, served by GitHub Pages (target domain: orangeca.se).

Plain HTML and CSS, no build step:

- `index.html`: the one-page site
- `assets/style.css`: styles, with light and dark themes
- `assets/logo.png`, `assets/favicon.svg`: brand assets

Preview locally:

```bash
python -m http.server 8000
```

To use a custom domain, add a `CNAME` file containing `orangeca.se` once the domain points at GitHub Pages.
