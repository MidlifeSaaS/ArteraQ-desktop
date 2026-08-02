# ArteraQ Desktop

A native macOS app for galleries, collection managers, and art advisors to
manage inventory, artists, consignments, and sales — fully offline, with your
data stored locally on your Mac.

Built with [Tauri](https://tauri.app) + [FrankenPHP](https://frankenphp.dev) +
SQLite. No account, no internet connection, and no subscription required to
use the app.

## Download

Latest release: **v0.4.2** (Apple Silicon / arm64)

Grab `ArteraQ_0.4.2_aarch64.dmg` from the
[Releases page](https://github.com/midlifesaas/ArteraQ-desktop/releases/latest).

> Apple Silicon (M1/M2/M3/M4) only for this release. Intel Mac support is not
> yet available.

## Installation

1. Download the `.dmg` from the link above.
2. Open it and drag **ArteraQ.app** to your Applications folder.
3. Launch ArteraQ from Applications (or Spotlight).
4. On first launch, the app initializes a local SQLite database — no setup
   required.

## Features

- Artwork inventory with images, valuations, and status tracking
- Artist records linked to inventory
- Consignment and sales workflows
- Local backup & restore (see **Settings → Backups**)
- Works fully offline — your data never leaves your Mac

## Data & Backups

Your data lives in:

```
~/Library/Application Support/com.arteraq.desktop/
```

Backups are created automatically before each update and can also be
triggered manually from **Settings → Backups**. Restoring from a backup is
the only recovery path if something goes wrong — there is no cloud copy.

## Updating

There is no auto-updater yet. To update to a new version:

1. Download the latest `.dmg` from the
   [Releases page](https://github.com/midlifesaas/ArteraQ-desktop/releases).
2. Quit ArteraQ if it's running.
3. Drag the new **ArteraQ.app** to Applications, replacing the old one.
4. Relaunch — any pending database migrations run automatically on startup,
   after a local backup is taken.

## Support

Found a bug or have a feature request? Open an issue on this repository.

## License

Licensed under the [GNU General Public License v3.0](LICENSE).
