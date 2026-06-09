# Unity Media — Landing Page

Static landing page (HTML + CSS + vanilla JS, no build step). Designed to be read and developed by Claude Code / any editor — every file is small.

## Quick start
- **View:** open `index.html` in a browser, or use VS Code → "Live Server".
- **Develop with Claude Code:** open this folder in VS Code and ask Claude Code to read `CLAUDE.md` first — it explains the whole structure.

## Structure
```
index.html              Page markup (all sections)
CLAUDE.md               Project brief for Claude Code (read this first)
css/
  01-tokens-base.css    Design tokens, reset, buttons, section heads
  02-header.css         Header + mobile menu
  03-hero.css           Hero
  04-sections.css       Trust, Why, Services, Coverage, Work, Results, Process, Testimonials, FAQ
  05-footer-forms.css   Lead form, footer, scroll reveal
  06-responsive.css     Responsive breakpoints
js/
  script.js             Interactions
images/                 Logos + hero + campaign photos
```

## Upload to GitHub
Upload the **contents of this folder** (the files and the `css/`, `js/`, `images/` folders) to your repo — **not** a zip. Then point Claude Code at the repo.

## Brand
Red `#E11B22` · Navy `#0C1E33` · Archivo (headings) + Manrope (body). Tokens live in `css/01-tokens-base.css`.
