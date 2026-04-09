# OpenEmu ES-DE Theme

## What This Is
An ES-DE (EmulationStation Desktop Edition) theme that replicates OpenEmu's dark, minimal, library-style UI. The goal is to use ES-DE as a frontend for standalone emulators (PCSX2, RPCS3, Dolphin, Cemu, Ryubing) while keeping the clean aesthetic the user loves from OpenEmu.

## Theme Structure
- `capabilities.xml` — declares variants, color schemes, aspect ratios, transitions
- `colors.xml` — 3 color schemes: Dark (default), OLED Black, Light
- `theme.xml` — main layout: system carousel view + gamelist views (grid/list)
- `aspect-ratio-*.xml` — layout overrides per aspect ratio (16:9, 16:10, 4:3, 21:9)
- `_inc/fonts/` — Inter font family (SIL Open Font License)
- `_inc/images/space.png` — 1x1 spacer tile for tinted backgrounds
- `_inc/systems/artwork/` — per-system background art (PNG, named by system ID)
- `_inc/systems/logos/` — per-system logos (SVG, named by system ID)
- `_inc/sounds/` — navigation sound effects (WAV)

## Variants
- `grid-cover` — grid of cover art (default, closest to OpenEmu)
- `grid-screenshot` — grid of screenshots
- `list-cover` — text list with cover art + metadata sidebar
- `list-basic` — plain text list

## Key Design Decisions
- Inter font chosen to match macOS/OpenEmu clean sans-serif feel
- Color palette extracted from OpenEmu: charcoal #1B1B1B background, blue #4A90D9 accent
- ES-DE cannot do a persistent sidebar (system+gamelist on one screen) — system view and gamelist are separate screens
- No blur/frosted glass in ES-DE theme engine — use pre-blurred images as workaround

## What Still Needs Doing
- Add system artwork PNGs to `_inc/systems/artwork/`
- Add system logo SVGs to `_inc/systems/logos/`
- Add navigation sound WAVs to `_inc/sounds/`
- Test in ES-DE and tune spacing/sizing
- Add per-system metadata XML files
- Consider adding badge icons for favorites/completed

## ES-DE Theme Docs
- Theme dev reference: https://gitlab.com/es-de/emulationstation-de/-/blob/master/THEMES-DEV.md
- System IDs list: https://gitlab.com/es-de/themes/system-metadata
- System logos: https://gitlab.com/es-de/themes/system-logos

## Tech Notes
- Theme format is pure XML, no CSS/JSON
- Two views: `system` (system selection) and `gamelist` (game list per system)
- Elements: grid, textlist, carousel, image, text, video, badges, rating, datetime
- Variables use `${varName}` syntax, colors are RRGGBBAA hex
- Install path: `~/.emulationstation/themes/es-de-openemu-theme/`
