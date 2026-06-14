# Team Secrets — Releases

Official downloads and over-the-air (OTA) update manifest for **Team Secrets**, a desktop
team credential manager (SOPS + age, git-synced).

## Download

Grab the latest installer for your OS from the [**Releases**](../../releases/latest) page.

| OS | File |
|----|------|
| macOS (Apple Silicon) | `Team Secrets_*_aarch64.dmg` |
| macOS (Intel) | `Team Secrets_*_x64.dmg` |
| Windows | `Team Secrets_*_x64_*.msi` |
| Linux | `team-secrets_*_amd64.AppImage` / `.deb` |

## First launch — unsigned build notice

These builds are **not code-signed** yet, so the OS will warn on first launch.

- **macOS**: right-click the app → **Open** → confirm. Or run
  `xattr -dr com.apple.quarantine "/Applications/Team Secrets.app"`.
- **Windows**: SmartScreen → **More info** → **Run anyway**.
- **Linux**: `chmod +x` the AppImage, or install the `.deb`.

## Updates

Once installed, Team Secrets checks this repo for updates automatically and can update in place
(Settings → About → Check for Updates). The signed `latest.json` manifest lives on the latest release.
