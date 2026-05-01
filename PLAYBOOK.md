# April Fifteenth Playbook

This file is the fast-start brief for any new agent session working on this site.

## What This Project Is

`April Fifteenth` is a standalone static website about a submarine descent to the Titanic.

It is not a template exercise anymore.
It should be treated as its own site, with its own mood, visual system, and repo.

## Non-Negotiable Intent

- solemn, atmospheric, historical
- educational but not museum-boring
- interactive without feeling gimmicky
- visually authored, not generic sci-fi
- not horror, not disaster-porn, not theme-park Titanic

## Core Experience

As the user scrolls:

- the submarine descends
- the water darkens
- the HUD and depth rail update
- fact cards pace out oceanography, biology, and Titanic history
- the page ends at the wreck site

The page should feel like a descent, not like stacked content sections.

## Current Priorities

1. Improve visual integration of generated art assets.
2. Preserve the current structure and interaction logic.
3. Add polish through selective image placement, not by cluttering the page.
4. Recheck desktop and mobile after visual changes.

## Current Active Assets

Already used in `index.html`:

- `images/reef-canyon-wall-left.png`
- `images/reef-canyon-wall-right.png`
- `images/reef-canyon-wall-deep-left.png`
- `images/bubble-overlay-soft.png`
- `images/bubble-wake-trail.png`
- `images/titanic-wreck-footer-transparent.png`
- `images/ocean-surface-light.jpg`
- `images/ocean-reef-texture.jpg`

## Assets Available For Future Use

- `images/coral-cluster-sheet.png`
- `images/rock-shelf-set.png`
- `images/reef-platform-coral.png`
- `images/titanic-wreck-panorama-dark.png`

## Art Direction Rules

- Prefer restraint over abundance.
- Do not turn the scene into a sprite collage.
- Use decorative assets as framing and depth cues, not as the main event.
- The submarine, HUD, and fact pacing should remain the focal system.
- Favor cool Atlantic blues, desaturated reef tones, pale stone ledges, muted rust.
- Anything too tropical, too colorful, too cute, or too gamey should be dialed back.

## What To Avoid

- cheesy Titanic iconography
- treasure / sharks / fantasy ruins / pirate aesthetics
- overusing coral sprites everywhere
- photoreal elements mixed carelessly with painterly assets
- replacing the scroll mechanic with a conventional landing-page structure
- bloated rewrites when selective tuning would solve the issue

## Best Next Moves

Good next steps:

- add a few midground shelf accents from `rock-shelf-set.png`
- use `reef-platform-coral.png` sparingly on ledges
- tune wall image scale, opacity, and crop until they feel embedded
- consider subtle footer sediment / seafloor blending around the Titanic footer art

Bad next steps:

- adding many more cards just because assets exist
- swapping the whole visual language to match another template
- rebuilding the page from scratch unless the user explicitly asks

## Technical Notes

- Main file: `index.html`
- No framework / no build step
- Fonts are local in `fonts/`
- Run locally with:

```bash
cd /Users/mybbor/Library/CloudStorage/Dropbox/websites/April15th.com
python3 -m http.server 4180
```

- View at:

```text
http://127.0.0.1:4180/
```

## Codex Session Note

There is no local `codex init` subcommand in this environment.

The working pattern for Codex is:

1. open the repo root
2. read `README.md`
3. read `PLAYBOOK.md`
4. inspect `index.html`
5. iterate with render checks

## If You’re Starting Fresh

Read these first:

- `README.md`
- `PLAYBOOK.md`
- `index.html`

Then identify:

- what assets are active
- what the page is doing well
- what single visual weakness should be improved next

Do not start by broadening scope.
Start by improving the weakest visible part without damaging the strongest parts.
