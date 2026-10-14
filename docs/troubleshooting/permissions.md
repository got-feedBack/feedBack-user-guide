# Permissions

Short answer: FeedBack may need permission to use your microphone/input device, read local files, or run as a desktop app.

## Microphone/Input Permission

If the app cannot hear input:

1. Check operating-system microphone/input privacy settings.
2. Confirm FeedBack is allowed.
3. Restart FeedBack after changing permission.
4. Re-select the input device.

## Windows

- SmartScreen may warn on first run.
- Privacy settings can block microphone access.
- Security software can quarantine new builds.

## macOS

- Check System Settings → Privacy & Security → Microphone.
- If FeedBack never asks for microphone access and is not in that list, update to the current build. Some older builds were missing the audio-input entitlement, so macOS denied input silently ([#289](https://github.com/got-feedBack/feedBack/issues/289)).
- If the app is blocked, see [macOS Install Notes](../install/macos.md).
- Restart after permission changes.

## Linux

- AppImage files may need executable permission.
- Audio access depends on the distribution's audio stack.
- Sandboxed environments may need explicit device access.

## Related Pages

- [Desktop Install Problems](desktop-install.md)
- [No Signal](no-signal.md)
- [Audio Input Problems](audio-input.md)

