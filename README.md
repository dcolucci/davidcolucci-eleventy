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
