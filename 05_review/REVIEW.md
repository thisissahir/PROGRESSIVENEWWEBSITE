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
Open `index.html` in a browser (needs internet — images load from the Wix CDN, scripts from CDNs).

## To deploy to Vercel (when approved)
1. Put the contents of `04_build/` in a folder / repo.
2. `vercel` (or import the repo in the Vercel dashboard). It deploys as a static site; `vercel.json` is included.
3. Share the *.vercel.app preview URL. Domain/DNS stays untouched until you decide.

## Open items / next passes
- Optional: self-host the images into `03_assets/images/` instead of hotlinking the Wix CDN (faster, independent of Wix).
- Optional: real contact form (needs a form endpoint) — currently call + SoundCloud CTAs.
- Apollo can generate a bespoke OG image + favicon set.
- Add /work, /studio detail pages if you want more depth later.

## Repo / deploy (added 2026-07-05)
- **GitHub repo:** https://github.com/thisissahir/PROGRESSIVENEWWEBSITE.git
- **Deploy target:** Vercel (connect this repo in the Vercel dashboard → auto preview/prod on push).
- **What to put at repo root:** the contents of `04_build/` — `index.html` + `vercel.json` at the top level.
- Standard flow going forward: Forge commits → push → Vercel deploys (preview on branch/PR, prod on main).
