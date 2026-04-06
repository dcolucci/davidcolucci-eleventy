# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

This is an [Eleventy (11ty)](https://www.11ty.dev/) static site project. Currently a fresh boilerplate with `@11ty/eleventy@^3.1.5` installed and no source files or config yet.

## Commands

No npm scripts are configured yet. Use the Eleventy CLI directly:

```bash
npx eleventy          # Build the site to _site/
npx eleventy --serve  # Build + start dev server with live reload
npx eleventy --watch  # Build + watch for changes
```

## Architecture

Eleventy's **defaults** apply until an `eleventy.config.js` is added:

- **Input**: project root (all `.html`, `.md`, `.njk`, `.liquid` files get processed)
- **Output**: `_site/` (git-ignored)
- **Template engines**: Nunjucks, Liquid, and Markdown are all available (installed as dependencies)

When a config file is added, it will export a function from `eleventy.config.js` (or `.eleventy.js`) that receives the `eleventyConfig` object and returns an optional `{ dir: { input, output } }` object.

## Design Color Palette

Sourced from `davidcolucci.com` CSS. Use these as the canonical colors for this project:

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

## Architecture

**Installed template/utility libraries** (available without extra installs):
- `nunjucks` — primary templating
- `liquidjs` — Liquid templating
- `markdown-it` — Markdown processing
- `gray-matter` — front matter parsing
- `luxon` — date/time formatting in templates
