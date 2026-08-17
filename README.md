# Free Fire Booyah Pass Asset Viewer

A static browser utility for browsing configured Free Fire Booyah Pass assets loaded from public CDN endpoints.

**Live Demo:** https://mohith-krishnaa.github.io/Bpasset/

> **Unofficial tool:** This project is independent of Garena. Asset IDs, paths and CDN behavior can change with game updates.

## Features

- Manual OB/version selection
- BP-specific views through URL parameters such as `?bp=93`
- Increment-based asset scanning
- Configured premium-title, prize, background and subtype asset views
- Individual asset download controls
- Lightweight dark UI
- No framework or build system required

## How it works

```text
OB / BP configuration
        ↓
Asset ID generation
        ↓
CDN request
        ↓
Available asset
        ↓
Preview / download
```

## Run locally

```bash
git clone https://github.com/mohith-krishnaa/Bpasset.git
cd Bpasset
```

Open the static entry page in a modern browser or serve the directory with a local HTTP server.

## Usage

1. Open the application.
2. Select the desired OB/version or BP view.
3. Review the configured asset categories.
4. Preview discovered assets.
5. Download individual assets when appropriate.

The exact patterns are implementation-specific and depend on current game data and configured CDN endpoints.

## Important technical limitation

The application runs entirely in the browser. Therefore the browser can inspect the external CDN requests.

**Frontend JavaScript cannot hide or securely proxy a CDN URL.** A backend/proxy would be required if URL abstraction were actually necessary.

## Limitations

- Asset availability depends on external CDN behavior.
- Game updates can change asset IDs, paths and availability.
- The tool does not guarantee complete discovery of historical or current BP assets.
- Third-party rate limits or blocking can affect scanning.

## Asset ownership

Free Fire, Booyah Pass, game artwork and related assets are property of their respective rights holders, including Garena. This repository provides source code for a browser utility and does not claim ownership of third-party assets.

Use external assets only where you have the necessary rights and permission.

## License

See `LICENSE` for the source-code licensing terms.

## Author

**Mohith Krishnaa** — [@mohith-krishnaa](https://github.com/mohith-krishnaa)
