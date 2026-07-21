# FeedBack User Guide

📖 **Live guide:** https://got-feedBack.github.io/feedBack-user-guide/

Public user-guide wiki for FeedBack.

This repository contains the public user-guide source for FeedBack. It is designed to work in two places:

- Rendered website: https://got-feedback.github.io/feedback-user-guide/
- GitHub browsing: [SUMMARY.md](SUMMARY.md)

The docs are written as portable Markdown so they can be handed to design, integrated into the upcoming website, or read directly from GitHub.

## Start Here

| Need | Page |
|---|---|
| New user setup | [Quick Start](docs/quick-start.md) |
| Common questions | [FAQ](docs/getting-started/faq.md) |
| Terms and acronyms | [Glossary](docs/getting-started/common-terms.md) |
| Install the app | [Install FeedBack Desktop](docs/install/index.md) |
| Set up audio input | [Audio Input Setup](docs/first-run/audio-input.md) |
| Add songs | [Import Songs](docs/songs/import.md) |
| Fix no input signal | [No Signal](docs/troubleshooting/no-signal.md) |
| Report a bug | [Reporting an Issue](docs/troubleshooting/report-issue.md) |

## Support Shortcuts

- [Support and diagnostics hub](SUPPORT.md)
- [Audio Input Problems](docs/troubleshooting/audio-input.md)
- [No Sound or Output](docs/troubleshooting/no-sound-output.md)
- [Calibration Problems](docs/troubleshooting/calibration.md)
- [Playback Problems](docs/troubleshooting/playback.md)
- [Plugin Problems](docs/troubleshooting/plugins.md)
- [Desktop Install Problems](docs/troubleshooting/desktop-install.md)
- [Performance and Crashes](docs/troubleshooting/performance-crashes.md)
- [Export Diagnostics](docs/first-run/export-diagnostics.md)

## Browse By Section

- [Getting Started](SUMMARY.md#getting-started)
- [Installing FeedBack](SUMMARY.md#installing-feedback)
- [First-Time Setup](SUMMARY.md#first-time-setup)
- [Songs and Library](SUMMARY.md#songs-and-library)
- [Playing and Practicing](SUMMARY.md#playing-and-practicing)
- [Tuning, Input, and Calibration](SUMMARY.md#tuning-input-and-calibration)
- [Plugins](SUMMARY.md#plugins)
- [Desktop Audio](SUMMARY.md#desktop-audio)
- [Song Files and feedpak](SUMMARY.md#song-files-and-feedpak)
- [Troubleshooting](SUMMARY.md#troubleshooting)
- [Advanced Users](SUMMARY.md#advanced-users)

## Local Preview

Recommended preview stack:

```bash
pip install mkdocs mkdocs-material
mkdocs serve
```

The published site is built by GitHub Actions using [mkdocs.yml](mkdocs.yml).

## Content Status

- Screenshot callouts are placeholders until design captures final UI.
- Release-specific claims should be checked against the final target build before launch.
- Root-level files such as this README are for GitHub browsing and support workflows.

## Editing Notes

- Keep pages task-first.
- Use plain user-facing language before introducing technical terms.
- Prefer "song file" on beginner pages; introduce "feedpak" on file-format pages.
- Add platform/version notes where behavior differs.
- Keep GitHub-browsing helper files at the repo root so MkDocs navigation stays clean.
