# Paradise.la — Wireframe

Static HTML wireframe for the Paradise.la website redesign. Built as a reference / handoff package for the designer working in Webflow.

## Files

- **`paradise-wireframe-v1.html`** — main page (home). 8 sections following the agreed sitemap: Home/Manifesto · Selected Work · Always On Mode · Craft Mode · Why Paradise · Team · Contact · Footer.
- **`paradise-project-axion.html`** — project detail page template (Axion Energy). Click-through destination from the Selected Work slider.

## What's included

- Intro animation (film tape mark + Paradise wordmark + loading counter), Vucko-inspired
- Smooth scroll via [Lenis](https://github.com/darkroomengineering/lenis) (CDN)
- Fullscreen project slider with auto-advance, prev/next, thumbnails
- Word-by-word text reveal on scroll (light → dark, left → right)
- Hero parallax, count-up stats, scroll progress bar
- Dark mode toggle (persists per browser via localStorage, also respects OS preference)
- Click-through from any slide to the project page
- Mobile responsive (breakpoint at 900px)
- All section markers in `[s.0##]` style matching Paradise's visual language

## How to view locally

Open either HTML directly in any modern browser. No build step needed.

## How to view online

Enable GitHub Pages on this repo (Settings → Pages → Source: main / root). The wireframe will be live at `https://USERNAME.github.io/REPO/paradise-wireframe-v1.html`.

## What's a placeholder

- The hero reel video — currently loading from Paradise's own CDN (`sujan-experience.b-cdn.net/campari.mp4`) with a Google sample as fallback. Swap with the final reel.
- Project thumbnails in the slider — animated gradients. Swap with real video previews.
- Team portraits — initials on gray gradients. Swap with B&W photographs.
- Director / photographer roster names in Craft Mode — generic placeholders.
- Project page gallery images — gradient placeholders.
- The film tape SVG in the intro — generic film strip. Swap with Paradise's actual tape grading mark.

## Notes for the designer

This wireframe is a **functional spec**, not a Webflow export. Webflow doesn't import HTML directly. Treat this as a reference for:
- Section structure and order
- Interaction patterns (intro, slider, scroll reveals, dark mode)
- Typography hierarchy (Mona Sans + Caveat as accent)
- Color system (CSS variables, light + dark palettes)

The complex JS-driven effects (intro animation, Lenis smooth scroll, fullscreen slider, text reveal, dark toggle) can be packaged as Custom Code Embeds inside Webflow — happy to extract those as standalone snippets on request.
