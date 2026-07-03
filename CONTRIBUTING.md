# Contributing to the FeedBack User Guide

Thanks for helping improve the FeedBack user guide.

## Where To Start

- Browse the current docs from [SUMMARY.md](SUMMARY.md).
- Use the [Page Template](docs/contributing/page-template.md) for new pages.
- Follow the [Style Guide](docs/contributing/style-guide.md).
- Check [Design Handoff](docs/contributing/design-handoff.md) before adding screenshots.

## Writing Rules

- Write for users first.
- Keep pages task-first.
- Use exact UI labels from the current app build where possible.
- Avoid promising features that have not shipped.
- Link to troubleshooting and diagnostics pages when a workflow can fail.
- Use "song file" on beginner pages before introducing "feedpak".

## Local Preview

```bash
pip install mkdocs mkdocs-material
mkdocs serve
```

## Pull Request Checklist

- Links are relative and work on GitHub.
- MkDocs navigation is updated when adding public pages.
- `SUMMARY.md` is updated when adding public pages.
- No screenshots contain private paths or uncleared artwork.
- Release-specific claims are verified against the target build.
