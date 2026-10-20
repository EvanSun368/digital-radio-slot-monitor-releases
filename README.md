# Digital Radio Slot Monitor — Releases

Public **binaries only** for [Digital Radio Slot Monitor](https://github.com/sunguangxian/digital-radio-slot-monitor).

The application source code stays in the **private** repository `sunguangxian/digital-radio-slot-monitor`.

## Downloads

Use [Releases](https://github.com/sunguangxian/digital-radio-slot-monitor-releases/releases) for Windows builds (for example `DigitalRadioSlotMonitor.exe`).

## Publish a new build

From a machine that has the packaged exe:

```bash
gh release create vX.Y.Z DigitalRadioSlotMonitor.exe \
  -R sunguangxian/digital-radio-slot-monitor-releases \
  --title "vX.Y.Z" \
  --notes "Windows single-exe build. Source: private repo sunguangxian/digital-radio-slot-monitor."
```

The in-app **Check for Updates** feature queries this repository's `/releases/latest` API (no token required).
