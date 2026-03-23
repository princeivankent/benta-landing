# Benta Landing Page

## Architecture
- Single-file app: all HTML, CSS, and JS are inline in `index.html`
- No build process — edit `index.html` directly; no npm, no bundler, no dev server
- Images live in `/images/`

## CSS Patterns
- Design tokens (colors, spacing, radius) defined in `:root` at top of `<style>`
- Scroll-reveal: `.reveal`, `.reveal-left`, `.reveal-right`, `.reveal-stagger` + JS IntersectionObserver (threshold: 0.12)
- Mobile nav: `.nav-links a:not(.nav-cta)` hides links but keeps CTA button visible
- Reverse rows: use `order: -1` on `.showcase-img`, NOT `direction: rtl` (causes layout bugs)

## Product Context
- Philippine retail POS app for sari-sari/tindahan owners
- Filipino terms in copy (*utang*, *tindahan*, *negosyo*) are intentional — do not translate
- App URL: https://app.bentaph.com
- Plans: Tindahan (₱799/mo), Negosyo, Kadena (₱2,999/mo)

## Git
- LF→CRLF warnings on Windows are expected and harmless
