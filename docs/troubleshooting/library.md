# Library Problems

Short answer: if songs are missing or stale, check the file location, supported format, and scan/rescan state.

## Symptoms

- Song does not appear.
- Metadata did not update.
- Duplicate song versions appear.
- Library scan appears stuck.

## Fixes To Try

1. Confirm the song file is inside the library folder shown in Settings → System → **Library folder path**.
2. Click the refresh button (⟳) in the Song Library, or **Rescan Library** in Settings → System.
3. After metadata edits, click **Full Rescan** in Settings → System. It clears the cache and re-imports everything.
4. Restart FeedBack.
5. Export diagnostics if the issue repeats.

## Changed the Library Folder but Old Songs Still Show

After changing the library folder path, Rescan may keep reading the previous folder until FeedBack restarts ([#1063](https://github.com/got-feedBack/feedBack/issues/1063)). Restart the app after changing the folder. If you run FeedBack in Docker, the `DLC_DIR` setting decides the folder: change the `/dlc` mount instead.

## Related Pages

- [Import Songs](../songs/import.md)
- [Scan and Rescan](../songs/rescan.md)

