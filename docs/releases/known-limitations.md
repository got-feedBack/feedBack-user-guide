# Known Limitations

This page lists current user-facing limitations in the 0.3.0 alpha builds.

## Current Known Issues

| Issue | Platform | Workaround |
|---|---|---|
| Input works in the Audio screen but stops when a song starts ([desktop#126](https://github.com/got-feedBack/feedBack-desktop/issues/126)) | Desktop | Open the Audio screen and click **Apply Device Settings** again. |
| Wrong microphone used after the input setup wizard ([desktop#45](https://github.com/got-feedBack/feedBack-desktop/issues/45)) | Desktop | Re-select the input on the Audio screen and click **Apply Device Settings**. |
| Song audio is silent in Windows exclusive mode ([desktop#89](https://github.com/got-feedBack/feedBack-desktop/issues/89)) | Windows | Use shared Windows Audio or ASIO for output. |
| Song audio plays from the system default device ([#754](https://github.com/got-feedBack/feedBack/issues/754)) | Linux | Route FeedBack to the right device in `pavucontrol`. |
| Crash at startup on PipeWire without ALSA MIDI hardware ([desktop#128](https://github.com/got-feedBack/feedBack-desktop/issues/128)) | Linux | The issue has an `LD_PRELOAD` workaround that disables ALSA MIDI. |
| No build for Intel Macs ([desktop#99](https://github.com/got-feedBack/feedBack-desktop/issues/99)) | macOS | None yet. Builds are Apple Silicon only. |

## General

- Some platform-specific audio issues require diagnostics to debug.
- Virtual audio devices can be confusing because the OS and FeedBack may select different inputs.
- Some library metadata depends on what is present in the song file.
- Some advanced routing features are desktop-only or planned.

## Audio Input

FeedBack can only score or tune correctly if it is listening to the intended input. If the selected device and the actual device differ, export diagnostics in the same session after reproducing the issue.

## Library Metadata

Some fields only appear when the song file includes them or when a local metadata feature has filled them in. Missing album, genre, track number, or cover art is not always a bug.

## Platform Differences

Desktop builds can expose native audio and routing features that are not available in browser-hosted setups. Windows, macOS, and Linux may also name or route devices differently.

## Plugin Coverage

Not every plugin supports every arrangement type. A guitar-focused view may not appear for drums, keys, or vocals.

<!-- Maintainer note: do not use this page as a bug graveyard. Keep it short, current, and linked to fixes or troubleshooting pages. Remove a row when its issue closes. -->
