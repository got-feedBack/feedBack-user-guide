# ASIO, WASAPI, and CoreAudio

Short answer: driver types are the operating-system audio paths FeedBack can use to reach your input or output device.

## Why This Matters

The same physical audio interface can appear more than once if the operating system exposes it through different driver paths. Choosing the wrong path can cause higher latency, missing channels, or the wrong device being opened.

## Driver Types

| Driver Type | Platform | Notes |
|---|---|---|
| Windows Audio (WASAPI) | Windows | The default. Works with most devices. In exclusive mode, song audio can go silent ([feedBack-desktop#89](https://github.com/got-feedBack/feedBack-desktop/issues/89)). |
| ASIO | Windows | Often preferred for low-latency audio interfaces. |
| CoreAudio | macOS | Standard macOS audio system. |
| ALSA | Linux | The default. PipeWire and PulseAudio show up here as the PulseAudio sound server device. |
| JACK | Linux | For JACK setups, including `pipewire-jack`. |

FeedBack does not have a separate PipeWire or PulseAudio driver type.

## Choosing an Input

1. Open the **Audio** screen.
2. Pick the **Input Device Type** (the driver path), then the device name that matches your hardware. Output has its own **Output Device Type**.
3. Pick the correct channel.
4. Click **Apply Device Settings**.
5. Confirm signal in the tuner or input meter.

## Common Problems

| Problem | Try This |
|---|---|
| Same interface appears twice | Pick by driver label, not only device name. |
| Channel is missing | Try another driver path for the same interface. |
| Latency is high | Try the low-latency driver path for your interface. |

## Related Pages

- [Audio Input Setup](../first-run/audio-input.md)
- [Audio Input Problems](../troubleshooting/audio-input.md)

