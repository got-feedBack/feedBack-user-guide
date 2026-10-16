# Windows Install Notes

Use this page for Windows-specific install and first-launch notes.

## Steps

1. Download the Windows `.msi` installer from the latest release.
2. Run the installer.
3. If Windows SmartScreen appears, see [If Windows Blocks the Installer](#if-windows-blocks-the-installer).
4. Launch FeedBack.

## If Windows Blocks the Installer

The Windows builds are not code-signed yet, so Windows SmartScreen may show "Windows protected your PC" when you run the installer or the Portable app. If you downloaded it from the official release page:

1. Click **More info**.
2. Click **Run anyway**.

If Smart App Control is on, it may block the app with no **Run anyway** button. In that case, Smart App Control has to be turned off in Windows Security → App & browser control → Smart App Control settings. This setting applies to every app on the PC, so decide whether that trade-off is right for you.

The maintainers are working on code signing for the Windows builds. Once the builds are signed, this warning should go away. Progress is tracked in [feedBack#118](https://github.com/got-feedBack/feedBack/issues/118).

## Audio Notes

Windows users may see more than one entry for the same interface because the same hardware can expose different driver paths, such as ASIO and WASAPI. Choose the entry that matches the driver path you intend to use.

## Common Problems

| Problem | Try This |
|---|---|
| The app will not start | Reinstall from the latest release and check antivirus quarantine. |
| The wrong input is selected | See [Audio Input Problems](../troubleshooting/audio-input.md). |
| Interface names look duplicated | Look for the driver label in parentheses. |

