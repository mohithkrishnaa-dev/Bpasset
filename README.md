# Free Fire Booyah Pass Asset Viewer

A static browser-based utility for browsing Free Fire Booyah Pass assets loaded dynamically from public CDN endpoints.

**Live Demo:** https://mohith-krishnaa.github.io/Bpasset/

## Features

- Manual OB/version selection
- BP-specific views through URL parameters such as `?bp=93`
- Increment-based asset scanning
- Browsing of configured premium-title, prize, background and subtype assets
- Individual asset download controls
- Lightweight black UI
- No framework or build system required

## How it works

```text
OB / BP configuration
        ↓
Asset ID generation
        ↓
CDN request
        ↓
Available assets
        ↓
Preview / Download
```

## Usage

1. Open the application in a modern browser.
2. Configure the OB/base URL used by the current implementation.
3. Select or open the desired BP view.
4. Review the discovered assets.
5. Download individual assets when needed.

The exact asset patterns are implementation-specific and depend on the configured CDN endpoints and current game data.

## Tech stack

- HTML
- CSS
- Vanilla JavaScript

## Limitations

- Asset availability depends on external CDN endpoints and their current behavior.
- CDN URLs are visible to the browser and cannot be hidden by frontend JavaScript.
- Game updates can change asset IDs, paths or availability.
- This tool does not guarantee that every historical or current BP asset is discoverable.

## Asset ownership and disclaimer

Free Fire, Booyah Pass, game artwork and related assets are the property of their respective rights holders, including Garena. This repository contains source code for a browser utility and does not claim ownership of third-party game assets.

Use external assets only where you have the necessary rights and permission.

## License

See the repository license for the source-code licensing terms.

## Author

**Mohith Krishnaa** — [@mohith-krishnaa](https://github.com/mohith-krishnaa)
