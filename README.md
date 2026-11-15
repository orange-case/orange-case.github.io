# orange-case.github.io

Static website for **The Orange Case**, served by GitHub Pages (target domain: orangeca.se).

Plain HTML and CSS, no build step:

- `index.html`: the one-page site
- `404.html`: not-found page, uses absolute `/assets/...` paths because GitHub Pages serves it for any path
- `assets/style.css`: styles, with light and dark themes
- `assets/logo.png`, `assets/favicon.svg`: brand assets (`logo.png` is the original and the fallback image)
- `assets/logo.webp`: optimised copy of the logo that the pages load first, via `<picture>`
- `assets/social-card.png`: 1200x630 link preview image referenced by `og:image`

Colours: `--orange` is for fills, the diagram and the glow. Orange text uses `--orange-text` and the primary button uses `--orange-btn`, so both meet WCAG AA in light and dark themes.

`logo.webp` and `social-card.png` are generated from `logo.png` with Pillow. Regenerate them if the logo changes.

Preview locally:

```bash
python -m http.server 8000
```

To use a custom domain, add a `CNAME` file containing `orangeca.se` once the domain points at GitHub Pages.
