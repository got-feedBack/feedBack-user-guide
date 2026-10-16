# Linux Install Notes

Use this page for Linux-specific install and first-launch notes.

## AppImage

1. Download the AppImage.
2. Make it executable.
3. Run it.

### Distributions Without AppImage Support

Some distributions (for example CachyOS) have no native AppImage support, so opening the file may not install or launch it. [Gear Lever](https://flathub.org/apps/it.mijorus.gearlever) can install it for you, without the terminal:

1. Download the `feedback-*.AppImage` file.
2. Install Gear Lever from your Software app (it is on Flathub).
3. Open Gear Lever once and complete its first-run steps.
4. Double-click the AppImage and let Gear Lever install it.
5. Launch FeedBack from your app menu.

## Debian or Ubuntu Package

1. Download the `.deb` package.
2. Install it with your package manager.
3. Launch FeedBack from your app menu or terminal.

## Audio Notes

Your distribution and audio stack determine which devices appear. If you use PipeWire, JACK, or PulseAudio routing, confirm that FeedBack receives the intended input before calibration.

