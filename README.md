# Nilo Labs — Landing Page

Official marketing website for Nilo Labs — a software boutique helping startups build and scale with technology.

## Stack

- Plain HTML + Tailwind CSS v4 (globally installed CLI)
- No package.json, no node_modules, no build tools in the repo

## Development

```bash
# Watch mode
tailwindcss -i src/input.css -o src/output.css --watch

# Production build
tailwindcss -i src/input.css -o src/output.css --minify
```

Then open `src/index.html` in a browser.

## Structure

```
src/
├── index.html       # Single-page site
├── input.css        # Tailwind directives + custom theme
├── output.css       # Generated (do not edit manually)
└── images/
    └── favicon/
```
