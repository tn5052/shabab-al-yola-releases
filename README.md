# Shabab AL Yola - Auto Update Releases

This is a **public repository** that hosts auto-update releases for the Shabab Database Manager desktop application.

## Purpose

The Shabab Database Manager is a private application, but it needs a public location to download updates from. This repository serves that purpose - it contains only the release files (installers and update manifests) that the auto-updater downloads.

## How It Works

1. When you push a version tag (e.g., `v1.0.1`) to the main repository, GitHub Actions automatically builds the app for Mac and Windows.
2. The signed update files are automatically published to this public repository.
3. When users open the app, it checks this repository for new updates and prompts them to install.

## Files

- **latest.json** - Update manifest that tells the app about the latest version
- **.dmg/.app.tar.gz** - macOS installers (Apple Silicon)
- **.msi/.nsis.zip** - Windows installers

All files are cryptographically signed to ensure they haven't been tampered with.

---

*This repository is automatically managed by GitHub Actions. Do not manually upload files here.*
