# OpenEmu Theme for ES-DE

A clean, dark, library-style theme for [ES-DE](https://es-de.org/) inspired by [OpenEmu](https://openemu.org/)'s iconic macOS interface.

## Features

- **Dark, minimal aesthetic** matching OpenEmu's charcoal palette
- **Grid view with cover art** as the default variant (just like OpenEmu's library)
- **3 color schemes**: Dark (default), OLED Black, Light
- **4 layout variants**: Grid Cover, Grid Screenshots, List Cover, List Basic
- **4 aspect ratios**: 16:9, 16:10 (MacBook), 4:3, 21:9 (Ultrawide)
- **3 font sizes**: Small, Medium, Large
- Smooth transitions and subtle animations

## Installation

1. Download or clone this repository
2. Place the `es-de-openemu-theme` folder in your ES-DE themes directory:
   - **macOS**: `~/.emulationstation/themes/`
   - **Linux**: `~/.emulationstation/themes/`
   - **Windows**: `%USERPROFILE%\.emulationstation\themes\`
3. Open ES-DE, go to **UI Settings > Theme Set** and select **OpenEmu**

## Variants

| Variant | Description |
|---------|-------------|
| Grid - Cover Art | Default. Grid of box art covers, closest to OpenEmu's library view |
| Grid - Screenshots | Grid of in-game screenshots |
| List - Cover Art | Text list with cover art preview and metadata on the right |
| List - Basic | Clean text-only list for fast navigation |

## Adding System Artwork

Place system artwork in `_inc/systems/artwork/` as PNG files named by system identifier (e.g., `nes.png`, `snes.png`, `psx.png`).

Place system logos in `_inc/systems/logos/` as SVG files (e.g., `nes.svg`, `snes.svg`).

## Credits

- Inspired by [OpenEmu](https://openemu.org/) by the OpenEmu Team
- Built for [ES-DE](https://es-de.org/) by Leon Stansfield
- Font: [Inter](https://rsms.me/inter/) by Rasmus Andersson (SIL Open Font License)

## License

MIT License - see [LICENSE](LICENSE) for details.
