# Linux Install Notes

Use this page for Linux-specific install and first-launch notes.

## AppImage

1. Download the AppImage.
2. Make it executable.
3. Run it.

## Debian or Ubuntu Package

1. Download the `.deb` package.
2. Install it with your package manager.
3. Launch FeedBack from your app menu or terminal.

## Audio Notes

Your distribution and audio stack determine which devices appear. FeedBack uses ALSA or JACK. On PipeWire or PulseAudio, pick ALSA and the PulseAudio sound server device, or JACK through `pipewire-jack`. Confirm that FeedBack receives the intended input before calibration.

