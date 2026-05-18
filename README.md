# Led Canvas

### SimHub LED authoring, packaged for early testers

Led Canvas is a SimHub plugin for building LED layouts, effects, telemetry
bindings, and custom device profiles from a visual editor.

This repository is the public release hub for Led Canvas installers and release
notes. The product source code is private; installer binaries are published as
GitHub Release assets when a build is ready.

## What's Included?

The current public target is `v0.2.0-alpha`, a free early tester build.

This alpha includes:

- Led Canvas SimHub plugin and WPF editor UI.
- Canvas Editor surface for LED layout work.
- Home effects: Static, Wave, Ripple, and Reactive.
- Event Animation authoring primitives.
- Telemetry binding UI and runtime paths.
- Custom device layout/profile tooling.
- Installer helper with payload hash verification.

This alpha does not include:

- Website account login.
- Payment, billing, or memberships.
- Device activation.
- Server-issued entitlements.
- Auto-update.
- Code signing or SmartScreen reputation.

## Download

Public installers are downloaded from the
[Releases](https://github.com/VISDE/LED_CANVAS/releases) page.

The first public alpha is being prepared. Until `v0.2.0-alpha` appears in
Releases with an attached `.exe` asset, there is no public installer download
from this repository.

Do not download Led Canvas from mirrored installers, reposted files, or the
automatic `Source code` archives.

## Installation

1. Close SimHub.
2. Download `LedCanvasSetup-v0.2.0-alpha.exe` from the GitHub Release asset when
   the release is published.
3. Verify the SHA256 hash shown in the release notes.
4. Run the installer.
5. If SimHub is not detected automatically, use the installer
   `/DIR="<SimHubRoot>"` option.

Installer helper logs are written under `<SimHubRoot>\_LedCanvasLogs\`.

## Verify The Installer

After downloading, run this in PowerShell from the download folder:

```powershell
Get-FileHash .\LedCanvasSetup-v0.2.0-alpha.exe -Algorithm SHA256
```

The expected hash will be listed in the matching release notes. If the hash does
not match exactly, do not run the installer.

## Current Alpha Checklist

The preparation checklist for the first alpha is here:

- [v0.2.0-alpha checklist](releases/v0.2.0-alpha-checklist.md)

## License

Led Canvas is proprietary software. The installer, plugin binaries, UI assets,
documentation, branding, and related materials remain the property of VISDE
unless a third-party license says otherwise.

You may not redistribute, repackage, mirror, sell, reverse engineer, decompile,
or modify Led Canvas without written permission.

See:

- [v0.2 alpha EULA](legal/v0.2-alpha-eula.md)
- [v0.2 alpha Privacy Notice](legal/v0.2-alpha-privacy.md)
- [Third-party notices](THIRD-PARTY-NOTICES.txt)

## About GitHub Source Archives

GitHub automatically shows `Source code (zip)` and `Source code (tar.gz)` links
on every release. In this repository those archives contain only public release
documents such as this README, legal notices, and release checklists.

They do not contain the private Led Canvas source code, and they do not include
uploaded installer assets unless a binary is mistakenly committed to this
repository.

## Support

For v0.2 alpha support, contact VISDE at `visdelht@gmail.com`.
