# Performance and Crashes

Short answer: performance problems can come from first-run model setup, heavy plugins, large libraries, graphics load, audio routing, or a bad song file.

## Symptoms

- App is slow to launch.
- Player stutters.
- UI freezes.
- A plugin makes the app sluggish.
- App closes unexpectedly.

## First Checks

1. Restart FeedBack.
2. Try a different song.
3. Disable non-essential plugins.
4. Close other audio or GPU-heavy apps.
5. If it happened after import, try removing the last imported song and rescanning.
6. Export diagnostics after reproducing.

## First Launch

The first launch can be slower than normal. If model downloads or cache setup are running, wait before force-closing unless the app is clearly stuck.

## Reset or Repair the Configuration

If problems started after an update, or settings seem stuck, the desktop app can reset its configuration. Open Settings → Plugins → **Audio Engine** → **Reset / repair configuration**:

| Option | What it clears |
|---|---|
| **Reset app settings & caches** | Audio device settings, window and UI preferences, Electron caches. Safe: rebuilt on next launch. |
| **Clear plugin state & cached Python deps** | Plugin enabled/disabled state, plugin data, and plugin-installed Python packages. Installed plugins stay. |
| **Full reset…** | Everything above. Optionally also removes installed plugins, the song library, and ML model caches. Only tick the song library box if you have a backup. |

## Reporting Details

- Platform and build.
- What you were doing.
- Whether it happens every time.
- Song and plugin involved.
- Diagnostics bundle.

## Related Pages

- [First Launch](../install/first-launch.md)
- [Plugin Problems](plugins.md)
- [Reporting an Issue](report-issue.md)
