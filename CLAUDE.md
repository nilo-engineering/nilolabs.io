# CLAUDE.md — Nilo Labs Landing Page

## Project overview
Static bilingual (pt-BR / en-US) landing page for Nilo Labs, a product & engineering consultancy for startups.

## Stack
- Plain HTML + Tailwind CSS v4 (CLI installed globally via mise, not in repo)
- No package.json, no node_modules, no bundler
- Single HTML entry point at `src/index.html`

## Build
```bash
# Generate CSS (required after editing input.css or HTML classes)
tailwindcss -i src/input.css -o src/output.css --minify
```

## Key conventions
- **Bilingual content**: `data-lang` attribute on `<html>` toggles `lang-pt` / `lang-en` visibility classes. Both languages live in the same HTML file.
- **Tailwind v4**: Config lives in `src/input.css` via `@theme` — there is no `tailwind.config.js`.
- **No JS frameworks**: All interactivity is vanilla JS at the bottom of `index.html`.
- **Form**: Contact form action is a Formspree placeholder — needs a real endpoint.
