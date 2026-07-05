# Progressive Collective — Staged for Review

**Status:** Draft v1, staged. Not published. No DNS/host change (as directed).

## What this is
A brand-new, premium dark-cinematic redesign of progressivecollective.in, built as a static
site for **Vercel**. Scroll drives the experience: hero parallax + staggered headline, a pinned
Mix & Master section where the line and image swap on scroll, a horizontal release catalogue
driven by vertical scroll, brand marquees, and reveal-on-enter throughout. Smooth scroll via Lenis,
animation via GSAP ScrollTrigger. **Logo kept identical** (the exact pclogo.png).

## Sections (mirrors the current site, rebranded)
Hero + client ticker → 01 Mix & Master (pinned) → 02 What we do → 03 Releases (horizontal) →
04 Recent brand work → 05 We are everywhere (brand marquee) → 06 What they say → Vision → 07 Contact/footer.

## All content is real
Pulled from the live site: 7 releases (real Spotify links + covers), 3 brand videos (Nippon/Bajaj/T-Series),
verbatim testimonials, real studio address + phone, real client roster.

## To preview locally
Serve the repo root (e.g. `python -m http.server`) and open it. **No internet needed** — every
image, font, and script is self-hosted under `assets/`. The only external URLs left are the
Spotify / SoundCloud / YouTube / Vimeo links users click to listen and watch.

## To deploy to Vercel (when approved)
1. The deployable site is the **repo root**: `index.html`, `vercel.json`, and `assets/`.
2. `vercel` (or import the repo in the Vercel dashboard). It deploys as a static site; `vercel.json` is included.
3. Share the *.vercel.app preview URL. Domain/DNS stays untouched until you decide.

## Open items / next passes
- Optional: real contact form (needs a form endpoint) — currently call + SoundCloud CTAs.
- Apollo can generate a bespoke OG image + favicon set.
- Add /work, /studio detail pages if you want more depth later.

## Repo / deploy (added 2026-07-05)
- **GitHub repo:** https://github.com/thisissahir/PROGRESSIVENEWWEBSITE.git
- **Deploy target:** Vercel (connect this repo in the Vercel dashboard → auto preview/prod on push).
- **What to put at repo root:** the contents of `04_build/` — `index.html` + `vercel.json` at the top level.
- Standard flow going forward: Forge commits → push → Vercel deploys (preview on branch/PR, prod on main).

## Deployed (2026-07-05)
- **Status:** LIVE on Vercel preview/prod (deployed from GitHub repo). Repo → Vercel pipeline confirmed working.
- Repo: https://github.com/thisissahir/PROGRESSIVENEWWEBSITE.git
- Going forward: Forge commits + pushes → Vercel auto-deploys. **Live URL: https://progressivenewwebsite.vercel.app/**
- Next passes (tomorrow): bespoke OG image + favicon (Apollo), optional contact form, /work + /studio detail pages, aesthetic tweaks.

## Self-hosted (2026-07-05, Sirius)
- **All render assets pulled off external CDNs into `assets/`** — nothing loads from Wix, cdnjs, jsdelivr, or Google Fonts anymore. Verified: local server showed zero external asset requests.
  - `assets/img/` — 13 photos/covers + `pclogo.png` (the exact identical mark) + a 128px `favicon.png`.
  - `assets/js/` — Lenis 1.0.42, GSAP 3.12.5, ScrollTrigger 3.12.5 (pinned, self-hosted).
  - `assets/fonts/` — Space Grotesk + Inter woff2 files + a localized `fonts.css` (`@font-face` → local).
- Favicon was a 21 MB PNG hotlink; replaced with a 4.9 KB `favicon.png` and the orphan deleted.
- Kept external (correctly — these are click destinations, not assets): Spotify, SoundCloud, YouTube, Vimeo, the live-site link.
- Rights note: images are the client's own uploads from progressivecollective.in (their own site) — cleared for the client's own rebuild.
