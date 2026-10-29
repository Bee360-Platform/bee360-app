# bee360 App – Releases

Official downloads of the bee360 desktop app for Windows and macOS.
This repository contains no source code – only the releases.

## Install

### Windows (winget)

```
winget install Bee360.Bee360            # Stable, for the current user (no admin rights)
winget install Bee360.Bee360.Preview    # Preview
winget install Bee360.Bee360 --scope machine   # Stable, machine-wide (UAC prompt / IT deployment)
```

### macOS (Homebrew)

```
brew install --cask bee360-platform/tap/bee360            # Stable
brew install --cask bee360-platform/tap/bee360@preview    # Preview
```

- Always use the **full name** (`bee360-platform/tap/…`). Homebrew 6 then trusts exactly this cask; `brew tap` plus the short name is refused for third-party taps.
- **Without admin rights** (standard user), install into your own Applications folder:

  ```
  brew install --cask --appdir=~/Applications bee360-platform/tap/bee360
  ```

  To make this the default, add `export HOMEBREW_CASK_OPTS="--appdir=~/Applications"` to `~/.zprofile`.
- `bee360` and `bee360@preview` cannot be installed at the same time; uninstall one before installing the other.

## Downloads

- Latest stable: https://github.com/Bee360-Platform/bee360-app/releases/latest
- All versions incl. preview: https://github.com/Bee360-Platform/bee360-app/releases

| File | Platform | Installs for |
|------|----------|--------------|
| `bee360_oneclick_installer_<version>_x64.msi` | Windows | current user, no admin rights |
| `bee360_deployment_installer_<version>_x64.msi` | Windows | all users (admin / software distribution) |
| `Bee360-app_<version>.dmg` | macOS | – |

## Channels

| Channel | GitHub           | Cadence       |
|---------|------------------|---------------|
| Stable  | Release (Latest) | when released |
| Preview | Pre-release      | weekly        |

## Support

Issues are disabled in this repository. For questions or problems with the app or the installation, please contact Bee360 support as described in the Support Guide: https://www.bee360.com/legal-documents

## Security

Please report vulnerabilities privately – see [SECURITY.md](SECURITY.md).
