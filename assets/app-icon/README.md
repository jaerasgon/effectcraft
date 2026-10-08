# Aurora app icon

**Creature:** a unicorn, as an engraved head-and-shoulders bust looking out of the tile.

**Style:** an ink engraving portrait in the Crafting Apps' owl-template framing (the FilmCraft owl):
full-bleed colour field, tight head-and-shoulders crop, the body running off the bottom and right edges.

**Tile:** 512 × 512 viewBox, rounded square `rx=112`, clipped; no border or roundel.

**Design:** aurora ribbons (green, violet, pink) over a night sky. Hand-authored SVG, no raster source.
Licence: see [LICENSE.txt](LICENSE.txt) (MIT OR Apache-2.0, like the repo).

## Files

| File | What |
|---|---|
| `aurora.svg` | master vector, traced at 2048 px (canonical) |
| `aurora-small.svg` | lighter vector (~350 KB), traced at 1024 px; also the web favicon |
| `aurora-1024.png` | 1024 px render |
| `aurora-macos-512.png` | runtime Dock icon on macOS, on Apple's 824/1024 grid |
| `aurora.icns` | macOS icon (Apple grid) |
| `aurora.ico` | Windows icon, 16–256 px; embedded in `aurora.exe` by `apps/aurora/build.rs` |
| `hicolor/<n>x<n>/apps/com.jaerasgon.aurora.png` | Linux icon theme, 16–512 px; the 256 px one is the runtime icon on Windows and Linux |
| `hicolor/scalable/apps/com.jaerasgon.aurora.svg` | Linux scalable icon |

App ID: `com.jaerasgon.aurora` (Wayland app ID, `packaging/linux/com.jaerasgon.aurora.desktop`).

## Regenerate

Copy a new `icon-master.svg` / `icon.svg` from craftrules `assets/app-icons/aurora/` over
`aurora.svg` / `aurora-small.svg`, then run `packaging/icons.sh` (needs `resvg`; `iconutil`
on macOS for the `.icns`). Copy `aurora-small.svg` to `apps/aurora-web/web/favicon.svg` too.
