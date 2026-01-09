# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Zed editor theme extension providing the "Sharp Solarized" theme family - sepia-toned, high-contrast light themes based on:
- [tinytinytinytiny/solarized-high-contrast-light](https://github.com/tinytinytinytiny/solarized-high-contrast-light) (original)
- [joshspicer/sharp-solarized](https://github.com/joshspicer/sharp-solarized) (fork)

## Theme Variants

- **Sharp Solarized**: Monochrome with red strings (`#b02402`), gray comments (`#767470`)
- **Sharp Solarized+**: Three-color with purple strings (`#471acc`), magenta comments (`#b41036`), green constants (`#147641`)

## File Structure

```
sharp-solarized-zed/
├── extension.toml          # Extension manifest for Zed
└── themes/
    └── sharp-solarized.json  # Theme definitions (schema v0.2.0)
```

## Development

### Local Testing
Copy the theme file to your Zed themes directory:
```bash
cp themes/sharp-solarized.json ~/.config/zed/themes/
```
Then select the theme in Zed settings.

### Theme Schema
Theme files follow https://zed.dev/schema/themes/v0.2.0.json

### Publishing
To publish to the Zed extension registry:
```bash
# From the repository root
zed extensions publish
```

## References

- [Zed Theme Documentation](https://zed.dev/docs/extensions/themes)
- [Zed Theme Schema](https://zed.dev/schema/themes/v0.2.0.json)
