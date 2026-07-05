# Progressive Collective

Brand-new, premium dark-cinematic static site for [progressivecollective.in](https://progressivecollective.in) — a 360° audio house serving brands and artists.

Scroll-driven experience: hero parallax, a pinned Mix & Master section, a horizontal release catalogue, brand marquees, and reveal-on-enter throughout. Smooth scroll via Lenis, animation via GSAP ScrollTrigger.

## Deploy on Vercel

This is a zero-config static site. `index.html` and `vercel.json` live at the repo root.

- **Vercel dashboard:** Import this repo — no build command or output directory needed. It deploys as a static site.
- **CLI:** run `vercel` from the repo root.

Vercel serves a `*.vercel.app` preview URL. Domain/DNS stays untouched until you decide to point it here.

## Repo layout

- `index.html`, `vercel.json` — the deployable site (root)
- `01_content-pack/` — source content
- `02_copy/` — copy deck
- `03_assets/` — visual system notes
- `04_build/` — build source (same as root files)
- `05_review/` — staged review copy + notes
- `brief.md` — build brief
