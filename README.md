# davidcolucci-eleventy

Personal site built with [Eleventy (11ty)](https://www.11ty.dev/), a static site generator.

## Tech

- **[Eleventy 3.x](https://www.11ty.dev/)** — static site generator
- **[Nunjucks](https://mozilla.github.io/nunjucks/)** — templating
- **Node.js** — runtime

## Requirements

- Node.js (v18 or higher recommended)

## Setup

```bash
npm install
```

## Commands

```bash
npm start      # Dev server with live reload at http://localhost:8080
npm run build  # Build to _site/
```

## Design Color Palette

Sourced from the legacy Refinery CMS powered `davidcolucci.com` CSS. Use these as the canonical colors for this project:

| Hex | Swatch |
|-----|--------|
| `#f5f5f5` | Off-white |
| `#2d2d2d` | Dark gray |
| `#767676` | Medium gray |
| `#aaa` | Lighter gray |
| `#ccc` | Very light gray |
| `#6196cc` | Muted blue |
| `#67cdcc` | Teal |
| `#f08d49` | Orange |
| `#f8c555` | Yellow |
| `#9C2626` | Dark red |

The color palette is also visualized in the [palette.html](/palette.html) file. Any updates to the color palette should be reflected in that file as well.

## Project Structure

```
src/
  _data/        # Global data files (content, site config)
  _includes/    # Layouts and partials
  assets/       # Static files (CSS, images, etc.)
  index.njk     # Homepage
_site/          # Build output (git-ignored)
eleventy.config.js
```
