# CLAUDE.md — Unity Media Landing Page

Project brief for Claude Code. Read this first.

## What this is
A single-page marketing landing page for **Unity Media** — an independent media representative running multi-market advertising campaigns across ASEAN & Oceania. Plain static site: HTML + CSS + vanilla JS. No build step, no framework.

## Run it
Open `index.html` in a browser (or use VS Code "Live Server"). Everything is local; works offline.

## File map (all files are small / readable)
```
index.html              Page markup — all sections in order (~370 lines)
css/
  01-tokens-base.css    Design tokens (:root variables), reset, buttons, section heads  ← edit colors/fonts/spacing HERE
  02-header.css         Sticky header + mobile menu
  03-hero.css           Hero section
  04-sections.css       Trust, Why, Services, Coverage, Work, Results, Process, Testimonials, FAQ
  05-footer-forms.css   Lead form, footer, scroll-reveal
  06-responsive.css     Tablet (<=1024) + mobile (<=720) breakpoints
js/script.js            Sticky header, count-up stats, scroll reveal, FAQ accordion, form handler
images/                 Logos + hero + 6 campaign photos
```

## Sections in `index.html` (top → bottom)
Header · Hero · Trust strip · Why Unity (4 cards) · Services (8 cards) · Coverage (6 regions) · Featured Work (6 cards) · Results (3 stats) · Process (6 steps) · Testimonials (3) · FAQ · Lead form · Footer.

## Design system
- **Colors:** red `#E11B22` (CTAs/accents), navy `#0C1E33` (dark sections/headings), ink `#16202B` (text), muted `#6B7785`, line `#E4E8EE`, soft `#F5F7FA`. All defined as CSS variables at the top of `css/01-tokens-base.css` — change them there, not inline.
- **Fonts:** Archivo (headings), Manrope (body), loaded from Google Fonts in `index.html`.
- **Radius:** 10 / 16 / 22px. **Content width:** 1200px. **Grid gap:** 28px.

## Conventions
- Edit design tokens in `css/01-tokens-base.css` `:root` — don't hardcode hex/sizes elsewhere.
- Keep class names descriptive (`.why-card`, `.work-card`, `.region-card`).
- Animations are progressive enhancement (content visible without JS); respect `prefers-reduced-motion`.

## Known TODOs (safe to work on)
- The contact form (`#contact-form` in `js/script.js`) is front-end only — wire it to a real backend/email service.
- Testimonials are representative placeholders — replace with verified client quotes.
- Add real contact details (email/phone) to the footer and form confirmation.

## Possible next steps you might be asked to do
- Convert to React/Next.js, Astro, or a WordPress theme.
- Add sections (pricing, team, case-study detail pages).
- Wire the form to Formspree / a serverless function / CRM.
