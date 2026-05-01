# April15th.com

Standalone static site for `April Fifteenth`, an interactive scroll-driven historical ocean descent to the Titanic.

## Project Summary

- Single-page static site.
- Main file: `index.html`
- No build system, no framework, no bundler.
- Visual structure: fixed underwater world + scroll-driven fact cards + HUD + depth rail.
- Tone: atmospheric, educational, historical, memorial rather than sensational.

## Core Concept

The page simulates a submarine descent through the ocean. As the user scrolls:

- the submarine descends
- the water darkens
- the HUD updates depth / pressure / zone / scale comparisons
- fact cards appear for oceanography, marine biology, and Titanic history
- the page ends at the Titanic wreck site

## Important Files

- `index.html`
- `fonts/blackout_midnight-webfont.woff`
- `fonts/blackout_sunrise-webfont.woff`
- `images/ocean-surface-light.jpg`
- `images/ocean-reef-texture.jpg`

## Currently Integrated Image Assets

These are already wired into `index.html`:

- `images/reef-canyon-wall-left.png`
- `images/reef-canyon-wall-right.png`
- `images/reef-canyon-wall-deep-left.png`
- `images/bubble-overlay-soft.png`
- `images/bubble-wake-trail.png`
- `images/titanic-wreck-footer-transparent.png`
- `images/ocean-surface-light.jpg`
- `images/ocean-reef-texture.jpg`

## Available But Not Yet Integrated

These exist in `images/` but are not currently used:

- `images/coral-cluster-sheet.png`
- `images/rock-shelf-set.png`
- `images/reef-platform-coral.png`
- `images/titanic-wreck-panorama-dark.png`

Recommended next use:

- use `rock-shelf-set.png` as sparse midground ledge accents
- use `reef-platform-coral.png` as selective shelf dressing
- use `coral-cluster-sheet.png` only in small doses to avoid a sprite-sheet feel
- keep `titanic-wreck-panorama-dark.png` as an alternate footer option, not a default replacement yet

## Current Visual State

What is working:

- HUD and depth rail
- mouse-tracking submarine behavior
- scroll-linked descent and fact pacing
- stronger title choice: `April Fifteenth`
- generated canyon wall art is a major improvement over the earlier SVG scenery

What still needs taste / iteration:

- side scenery may still need scale / opacity tuning
- some remaining abstract wall geometry may need to be reduced or removed
- midground reef detailing is still intentionally light
- mobile visual QA should be rechecked after any art changes

## Content / Research Notes

The page already includes source-backed stops covering:

- pelagic zones and light loss
- pressure scaling
- marine snow
- mesopelagic biomass
- black seadevil anglerfish
- vampire squid
- crown jelly
- Ahmed Gabr deepest scuba dive
- Grand Canyon depth comparison
- Cuvier's beaked whale depth record
- global conveyor belt / ancient deep water
- Titanic sinking, discovery, and wreck-site context

Primary sources are linked in the Sources section of `index.html`.

## Local Development

Serve locally from this folder:

```bash
cd /Users/mybbor/Library/CloudStorage/Dropbox/websites/April15th.com
python3 -m http.server 4180
```

Then open:

```text
http://127.0.0.1:4180/
```

For screenshots / QA, Playwright has been used successfully against the local server.

## Git

This folder is its own git repo.

Initialize status:

```bash
git status
```

If you want the first commit:

```bash
git add .
git commit -m "Initial April Fifteenth site extraction"
```

## Guidance For A New Agent Session

If continuing work here, prioritize in this order:

1. Improve visual integration of generated image assets without turning the page into a collage.
2. Keep the site solemn and authored; avoid theme-park Titanic aesthetics.
3. Preserve the scroll mechanic, HUD, and educational structure.
4. Prefer selective image layering over large structural rewrites.
5. Re-render in browser after every significant visual change.

## Origin

This project was extracted from the broader `brute-design` template workspace and is now intended to evolve as its own standalone site.
