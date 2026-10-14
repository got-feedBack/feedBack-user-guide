# Reporting an Issue

Short answer: include your build, platform, steps to reproduce, expected result, actual result, screenshots, and diagnostics.

## Good Bug Report Shape

```text
Build:
Platform:
Device/input:
What I expected:
What happened:
Steps to reproduce:
Screenshots/video:
Diagnostics bundle:
```

## Where to Report

- Desktop app problems (installing, updating, audio devices, crashes): [feedBack-desktop issues](https://github.com/got-feedBack/feedBack-desktop/issues).
- Everything else (library, playing, scoring, songs, the web app): [feedBack issues](https://github.com/got-feedBack/feedBack/issues).
- A specific plugin: that plugin's own repository (`got-feedBack/feedBack-plugin-<name>` for official plugins).

Search the open issues first. Your problem may already have a workaround.

## Before Reporting

1. Try the relevant troubleshooting page.
2. Reproduce in a fresh session if possible.
3. Export diagnostics in the same session after reproducing.

## Desktop Debug Log

For audio or crash problems, a debug log helps a lot. Start the desktop app with `--verbose` (or set the environment variable `SLOPSMITH_DEBUG=1`). FeedBack then writes `slopsmith-debug.log` to the app's logs folder, including native audio engine messages. Attach it with the diagnostics bundle.

## Related Pages

- [Export Diagnostics](../first-run/export-diagnostics.md)
- [Audio Input Problems](audio-input.md)
- [Library Problems](library.md)

