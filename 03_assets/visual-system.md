# Progressive Collective — Visual System (Apollo)
Direction: **premium, dark, cinematic recording-studio.** Expensive, restrained, tactile. The upgrade from the current bright-orange Wix look is a near-black, high-contrast, editorial space where the work (covers, brand logos, waveforms) is the colour.

## Palette (tokens)
- --pc-void:  #08080A   (page base, near-black)
- --pc-ink:   #101013   (raised surfaces / cards)
- --pc-line:  rgba(255,255,255,.10)  (hairlines)
- --pc-fog:   #9A9AA2   (muted text)
- --pc-bone:  #F4F1EA   (primary text / warm off-white)
- --pc-amber: #E8A04B   (single accent — a molten amber nod to the old orange, now premium/gold)
- --pc-amber-deep: #C7761F
- Accent used sparingly: CTAs, active states, waveform, hairline glows. 60-30-10: ~60% void, 30% ink/bone, 10% amber.

## Type
- Display: **Space Grotesk** (700/500) — big, tight, modern studio.
- Body/UI: **Inter** (400/500) — clean, legible.
- Huge hero type (clamp to ~12vw), generous negative space, uppercase micro-labels with letter-spacing.

## Texture / feel
- Subtle film grain overlay + faint vignette for cinematic depth.
- Hairline dividers, number-tagged sections (01 / 02 …), monospaced micro-labels.
- Rounded-none to 6px max; premium = sharp + spacious, not bubbly.

## Motion (the brief's core: scroll alters image + text)
- Smooth scroll (Lenis) + GSAP ScrollTrigger.
- Hero image parallax + slow scale; headline words rise/stagger in.
- Pinned "Mix & Master" section where the line changes ("Crystal clear mixes." → "Super loud masters.") as the image swaps.
- Releases: horizontal scroll gallery driven by vertical scroll.
- Brand logos: infinite marquee.
- Section reveals: clip-path / translate / fade on enter. Respect prefers-reduced-motion.

## Logo (LOCKED)
Use the client's exact pclogo.png — never redraw or recolor. Small in nav, larger in footer. On dark it reads as-is.

## FAIL-gate check
Amber lives on large/meaningful surfaces + accents (not just buttons); real covers & brand logos carry the colour; one consistent system; fast (lazy-load images, next-gen from Wix CDN); legible on mobile; logo used, not redrawn.
