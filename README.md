# Digital Radio Slot Monitor — Releases

Public **binaries only** for [Digital Radio Slot Monitor](https://github.com/EvanSun368/digital-radio-slot-monitor).

The application source code stays in the **private** repository `EvanSun368/digital-radio-slot-monitor`.

## Downloads

Use [Releases](https://github.com/EvanSun368/digital-radio-slot-monitor-releases/releases) for Windows builds (for example `DigitalRadioSlotMonitor.exe`).

## Publish a new build

Preferred path: create the release (with assets) on the **private** repo, then run Actions workflow `sync-public-release` (copies uploaded binaries here).

Manual fallback from a machine that has the packaged exe:

```bash
gh release create vX.Y.Z DigitalRadioSlotMonitor.exe \
  -R EvanSun368/digital-radio-slot-monitor-releases \
  --title "vX.Y.Z" \
  --notes "Windows single-exe (Qt). Source: private repo EvanSun368/digital-radio-slot-monitor."
```

The in-app **Check for Updates** feature queries this repository's `/releases/latest` API (no token required).
