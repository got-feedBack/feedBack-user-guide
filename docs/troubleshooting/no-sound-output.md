# No Sound or Output

Short answer: if FeedBack plays but you hear nothing, check output device, system volume, app volume, song audio, and plugin routing.

## First Checks

1. Confirm your speakers/headphones work outside FeedBack.
2. Check system volume and mute state.
3. Check FeedBack volume or mixer controls.
4. Try another song.
5. Restart FeedBack.
6. Check whether a plugin is muting or rerouting audio.

## Desktop Audio Checks

- Confirm the expected output device.
- If using an audio interface, confirm the hardware output and monitor level.
- If using advanced routing, simplify to the default output and test again.

## Song-Specific Checks

| Symptom | Possible Cause |
|---|---|
| One song is silent | Song may be missing audio or using unsupported audio. |
| Stems are silent | Stem mixer levels may be down. |
| Preview works but player is silent | Player route or plugin route may differ. |
| Song audio plays from the system default device instead of your chosen output (Linux) | Known issue ([#754](https://github.com/got-feedBack/feedBack/issues/754), [#214](https://github.com/got-feedBack/feedBack/issues/214)). Route FeedBack to the right device in `pavucontrol`. |
| Song audio is silent but your guitar is heard (Windows, exclusive mode) | Known issue ([feedBack-desktop#89](https://github.com/got-feedBack/feedBack-desktop/issues/89)). Switch the output to shared Windows Audio or to ASIO. |

## Reporting Details

- Platform.
- Output device.
- Whether other apps make sound.
- Whether all songs or one song fail.
- Screenshot of volume/mixer state if relevant.

## Related Pages

- [Playback Problems](playback.md)
- [Desktop Audio](../desktop-audio/index.md)

