# La Zagaleta Mansion: an AI-built luxury property landing page

An immersive, motion-led landing page for a newly built mansion in La Zagaleta, Benahavís (Costa del Sol, Spain), designed and built end to end by directing an AI model (Claude, by Anthropic). It is part of my applied AI portfolio: a working example of how I use AI to turn a short brief into a shipped and reviewed result.

**Live page:** https://asadravian.github.io/landing-page-la-zagaleta-mansion/

> Independent concept build. Not affiliated with or commissioned by Realista. Listing details and photography belong to Realista, Marbella (listing ref. 52595).

## The brief

One line and a link: build a highly immersive, premium landing page for a luxury mansion sale using HTML, Tailwind CSS and GSAP, drawing every detail and image from a public property listing.

## How it was made

| Step | What happened | Who |
| --- | --- | --- |
| 1. Specify | Before any code, the AI read the live listing and turned the brief into a detailed build specification covering facts, art direction, page choreography, motion and a quality bar. | AI drafted, I reviewed |
| 2. Ground | Every figure on the page (price, 8 bedrooms, 9 bathrooms, 1,380 m² built, 6,847 m² plot, room layout, agents) comes from the listing. Invented facts were ruled out from the start. | AI, checked by me |
| 3. Build | The AI produced the page from the specification and ran syntax and structure checks before handing it over. | AI |
| 4. Review | I tested it in the browser and fed back what I saw. Three rounds of fixes followed. | Me, then AI |
| 5. Systemise | The lessons from review were folded into a reusable specification for future property pages. | AI drafted, I approved |
| 6. Ship | Deployed with GitHub Pages. | AI pushed, I configured hosting |

### What human review caught

1. **A photo viewer that would not close.** The gallery viewer appeared over the page on load because a layout rule overrode its hidden state. One global rule fixed it, along with a "thank you" message that was showing before the form was sent.
2. **A navigation bar that was hard to read.** The menu text blended with the photography behind it. It now uses solid champagne-gold text over a soft shade, switching to a dark frosted bar after scrolling.
3. **Wrong market detail.** The phone field showed a UK example number on a Spanish listing. It now shows a Spanish format while still accepting any country code.

All three became standing rules for future builds.

### A limitation, stated plainly

The AI could not view the listing photos in its build environment, so it matched photos to sections by the listing's gallery order rather than by what each photo shows. It said so up front, and the build was structured so any photo can be reassigned in seconds.

## What this demonstrates

- **Specification before generation:** a structured brief with a quality bar produces better first drafts than an open request.
- **Grounding:** facts come from a source, and anything not in the source stays off the page.
- **Human in the loop:** the model builds fast, while a person judges how it looks and feels.
- **Turning one-off work into a reusable asset:** lessons from one project become rules for the next.
- **Honesty about limits:** what the AI could not verify is stated openly.

These are the same habits I bring to AI adoption and enablement work with teams.

## The page

- Counter preloader with a curtain reveal into the hero
- Hero photo with masked headline reveal and scroll parallax
- Manifesto paragraph that brightens word by word as you scroll
- Key figures that count up on entry
- Pinned "arrival" sequence with slit-to-full-frame reveals
- Pinned horizontal walk through each level of the house
- Stacked master suite cards and a lower-level amenity list where photos follow the cursor
- Panning grounds panorama, stylised location map and specification grid
- 40-photo gallery with a keyboard-accessible viewer
- Private viewing form with inline validation
- Simplified motion on phones and a fully static page for visitors who prefer reduced motion

## Built with

HTML, Tailwind CSS, GSAP with ScrollTrigger, Lenis smooth scrolling and GitHub Pages.

## Rights

Copyright © 2026 Muhammad Asadullah. All rights reserved. The code is published for viewing as a portfolio piece only and may not be copied, reused or redistributed without written permission. See [LICENSE](LICENSE). Listing information and photography remain the property of Realista.

## Author

Muhammad Asadullah, applied AI and AI adoption. GitHub: [@asadravian](https://github.com/asadravian)
