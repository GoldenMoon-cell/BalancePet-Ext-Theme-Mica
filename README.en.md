# BalancePet themes

Every BalancePet **theme** lives here: one directory per theme, packaged and attached to this repository's releases, with `catalog.json` as their catalogue.

| Theme | Materials | Notes |
| --- | --- | --- |
| [BalancePet Mica](themes/balancepet-mica) | Mica / Mica Alt / Solid | System Mica, Fluent controls, teal accent |
| [BalancePet Acrylic](themes/balancepet-acrylic) | Acrylic / Solid | Translucent palette built for acrylic: low-opacity surfaces, bright edges, stronger shadows |

## Installing

1. Download a theme from [Releases](https://github.com/GoldenMoon-cell/BalancePet-Themes/releases)
2. Import the ZIP under Settings - Appearance, or drop it on Settings - Extensions
3. Choose it under Settings - Appearance - Current theme

Requires BalancePet **1.0.0** or newer. The host applies the material through Windows APIs; a theme only declares which materials it supports.

## Building one

Copy `themes/balancepet-mica`, change the `id` and names in `manifest.json`, change the colours in `theme.json`, then run `tools/package-theme-extension.ps1`. Colours are `#RRGGBB` or `#AARRGGBB`; `backdrops` lists the supported materials, and `solid` is always available as the fallback.

## License

MIT