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

These builds are **not notarized**, so the OS warns on first launch.

### macOS — if you see "Team Secrets is damaged and can't be opened"

The app is **not** damaged. macOS shows this because of the quarantine flag, and
**right-click → Open / "Open Anyway" do not clear it.** Run this once:

```sh
xattr -dr com.apple.quarantine "/Applications/Team Secrets.app"
```

(Drag the app into `/Applications` first.) Then open it normally.

### Windows

SmartScreen → **More info** → **Run anyway**.

### Linux

`chmod +x` the AppImage, or install the `.deb`.

## Updates

Once installed, Team Secrets checks this repo for updates automatically and can update in place
(Settings → About → Check for Updates). The signed `latest.json` manifest lives on the latest release.
