# macOS Install Notes

Use this page for macOS-specific install and first-launch notes.

## Steps

1. Download the macOS `.pkg` installer from the latest release. Builds are for Apple Silicon (M1 or newer) only.
2. Open the `.pkg` and follow the installer.
3. Launch FeedBack.
4. When macOS asks, allow FeedBack to use the microphone. FeedBack needs this to hear your instrument, even through an audio interface.

The release also has a Portable `.zip`. Unzip it and move the app to Applications.

## If macOS Blocks the App

Nightly and test builds are signed but not notarized, so macOS may refuse to open them. Clear the quarantine flag once, then open the app again. If you put the app somewhere other than Applications (for example, after unzipping the Portable `.zip`), use that path instead:

```bash
xattr -dr com.apple.quarantine "/Applications/fee[dB]ack.app"
```

## Audio Notes

macOS uses CoreAudio. If you use a virtual device such as BlackHole, confirm that FeedBack is actually listening to that device before calibrating or scoring.

## Common Problems

| Problem | Try This |
|---|---|
| FeedBack hears the internal mic instead of your selected device | See [Audio Input Problems](../troubleshooting/audio-input.md). |
| A virtual device appears but does not work | Re-select the device in FeedBack and verify macOS Sound settings. |
| No input and no microphone prompt | Allow FeedBack in System Settings → Privacy & Security → Microphone. See [Permissions](../troubleshooting/permissions.md). |

