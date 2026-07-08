# pixelboreal portfolio site

This repo IS the live website: GitHub Pages serves `index.html` at
https://fct4r8jk6f-cmyk.github.io/pixelboreal/ — every push to main redeploys
automatically (allow ~1 minute).

## What this site is
The public face of **pixelboreal**, a faceless bilingual web studio in Montréal
run by Nicholas. It exists to make the three Fiverr gigs credible and must never
reveal his name, face, or personal details. "pixelboreal" is always lowercase.

## Hard rules
- **Single file, no build step.** Everything (CSS/JS/SVG logo) stays inline in
  `index.html`. No frameworks, no CDNs, no external requests. This constraint is
  part of the sales pitch ("one file, loads instantly — like everything I ship").
- **Fully bilingual EN / fr-CA.** Every visible string exists in BOTH `I18N.en`
  and `I18N.fr` in the script block. French is Québec French (fr-CA), never
  France-French. Never add copy in one language only.
- **Both themes work.** Dark (default) and light via CSS custom properties on
  `[data-theme]`. Check contrast in both after any style change.
- **Palette:** sky #0E1726, panel #162338, line #2E405C, mint #3FE0A6 (primary
  accent), cyan #46C8F0, purple #8B6FE8, spruce #26845C, snow #E9F2FA. Light
  theme overrides live in the same `:root`/`[data-theme="light"]` blocks.
- Respect `prefers-reduced-motion`; keep focus states visible.

## Links that must stay correct
- Fiverr profile: https://www.fiverr.com/awouleh
- Gig 1 (bug fixes): /awouleh/fix-bugs-on-your-website-fast-at-a-flat-price
- Gig 2 (bilingual sites): /awouleh/build-a-fast-bilingual-website-in-english-and-french
- Gig 3 (fr-CA localization): /awouleh/localize-your-website-into-real-quebec-french-fr-ca
- Featured work (Perch demo): https://fct4r8jk6f-cmyk.github.io/perchapp/

## Wider context (for cloud sessions with no local memory)
The business's canonical docs live on Nicholas's machine at
`C:\Users\nicho\Documents\pixelboreal\` (not in this repo). That parent folder is
also the dedicated LOCAL Claude Code project for pixelboreal (own CLAUDE.md +
memory); this repo checkout lives inside it at `site\`. Cloud sessions here handle
website edits only — Fiverr/business ops and browser automation happen in local
sessions from that parent folder. Gig prices as of
2026-07: bug fixes $60/130/280 · bilingual sites $150/420/850 · fr-CA
localization $120/260/520. If copy references prices, keep the "from $X" values
in sync with the `c1_tag`/`c2_tag`/`c3_tag` i18n keys (both languages).
