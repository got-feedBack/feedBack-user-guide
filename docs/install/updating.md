# Updating FeedBack

Short answer: on Windows and macOS, FeedBack updates itself. Pick an update channel in Settings → System → App updates, then restart when an update is ready.

## App Updates on Windows and macOS

FeedBack checks for a new build at launch and every few hours, and downloads it in the background.

1. Open Settings → System → **App updates**.
2. Pick a channel: Stable, Release candidate, Beta, Alpha, or Nightly. Pick the one that matches the build you installed, or a newer one if a tester or maintainer asks you to.
3. Click **Check for updates** to check right away.
4. When the status says the update is ready, the button changes to **Restart now**. Click it to install.

To install a specific older build, download it from the FeedBack Desktop releases page instead.

## App Updates on Linux

- The AppImage updates itself on the Nightly channel.
- The `.deb` package does not update itself. Download the new `.deb` from the releases page and install it over the old one.

## Plugin Updates

1. Open Settings → Plugins → **Plugin updates**.
2. Click **Check for Updates**.

## Before Updating

- Keep a backup of song files you edited by hand.
- If you are testing a specific build, do not update unless your tester instructions say to.

## Related Pages

- [0.3.0 Notes](../releases/0-3-0.md)
- [Known Limitations](../releases/known-limitations.md)
