# Progressive Collective

Brand-new, premium dark-cinematic static site for [progressivecollective.in](https://progressivecollective.in) — a 360° audio house serving brands and artists.

Scroll-driven experience: hero parallax, a pinned Mix & Master section, a horizontal release catalogue, brand marquees, and reveal-on-enter throughout. Smooth scroll via Lenis, animation via GSAP ScrollTrigger.

**Fully self-hosted** — every image, font, and script lives in `assets/`. Nothing loads from an external CDN, so the site is independent of Wix, cdnjs, jsdelivr, and Google Fonts. (The Spotify / SoundCloud / YouTube / Vimeo links are click-through destinations, not loaded assets.)

## Deploy on Vercel

This is a zero-config static site. `index.html`, `vercel.json`, and `assets/` live at the repo root.

- **Vercel dashboard:** Import this repo — no build command or output directory needed. It deploys as a static site.
- **CLI:** run `vercel` from the repo root.

Vercel serves a `*.vercel.app` preview URL. Domain/DNS stays untouched until you decide to point it here.

## Repo layout

- `index.html`, `vercel.json`, `assets/` — the deployable, self-hosted site (root)
  - `assets/img/` — photos, covers, logo (`pclogo.png`), favicon
  - `assets/js/` — Lenis, GSAP, ScrollTrigger (pinned versions)
  - `assets/fonts/` — Space Grotesk + Inter woff2 files and `fonts.css`
- `01_content-pack/` — source content
- `02_copy/` — copy deck
- `03_assets/` — visual system notes
- `04_build/` — build source (same as root files)
- `05_review/` — staged review copy + notes
- `brief.md` — build brief
