# CLAUDE.md

## Project Overview

Static GitHub Pages site for the **GeodesicNVS** paper (CVPR 2026). Based on the Nerfies project page template.

## Development

No build system, no tests, no linting. To preview locally:

```sh
python3 -m http.server
```

Or open `index.html` directly in a browser.

## Tech Stack

- **Bulma CSS** (0.9.1) — layout and components
- **jQuery** (3.5.1, CDN) — DOM manipulation
- **Bulma Carousel / Bulma Slider** — image carousels (`static/js/bulma-carousel.min.js`, `static/js/bulma-slider.min.js`)
- **FontAwesome** + **Academicons** (CDN) — icons

## Key Files

| File | Purpose |
|------|---------|
| `index.html` | Main (and only) page — all content lives here |
| `static/css/index.css` | Custom styles |
| `static/js/index.js` | Navbar burger toggle + carousel/slider initialization |

## Image Assets

Organized under `static/images/` in subdirectories:

- `teaser/` — teaser figures
- `d2d_fm/` — D2D flow matching results
- `geodesic_fm/` — geodesic flow matching results
- `gso30_nvs/` — GSO30 novel view synthesis comparisons
- `path_figure/` — path/trajectory figures
- `framework.png` — method overview

## Important

`geodesicNVS_arxiv/` contains LaTeX source for the paper. It is gitignored — **never commit or modify** files in that directory.

## Deployment

Push to `main` branch. GitHub Pages serves automatically.
