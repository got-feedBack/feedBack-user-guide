# Desktop Install Problems

Short answer: if the desktop app will not install or launch, confirm the correct package, OS permissions, and whether security software blocked the app.

## First Checks

1. Download the latest package for your platform.
2. Confirm the package matches your CPU/OS.
3. Reinstall.
4. Restart the machine if the installer or audio driver path changed.
5. Check security prompts or quarantine.

## Windows

- SmartScreen may warn on first run. See [If Windows Blocks the Installer](../install/windows.md#if-windows-blocks-the-installer).
- Antivirus tools can quarantine new builds.
- Audio interfaces may need vendor drivers.

## macOS

- Builds are for Apple Silicon (M1 or newer) only. Intel Macs are not supported yet.
- If macOS refuses to open the app, see [If macOS Blocks the App](../install/macos.md#if-macos-blocks-the-app).
- Confirm microphone permissions if setup cannot hear input.

## Linux

- AppImage files may need executable permission. On distributions without native AppImage support, see [Distributions Without AppImage Support](../install/linux.md#distributions-without-appimage-support).
- Package dependencies may vary by distribution.
- Audio routing depends on the local audio stack.

## Reporting Details

- OS version.
- Package filename.
- Installer error text.
- Screenshot of the failure.

## Related Pages

- [Install FeedBack Desktop](../install/index.md)
- [First Launch](../install/first-launch.md)

