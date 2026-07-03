# Manifest Metadata

Short answer: `manifest.yaml` is the index for a feedpak. It tells FeedBack what the song is and where the related files are.

## What The Manifest Does

- Stores title, artist, album, and other catalog fields.
- Points to arrangement files.
- Points to audio stems, lyrics, cover art, and side files.
- Declares feedpak format version where present.

## Common Fields

| Field | Meaning |
|---|---|
| title | Song title. |
| artist | Recording or performing artist. |
| album | Album or release name. |
| year | Year when known. |
| arrangements | Playable chart files. |
| stems | Audio files. |
| lyrics | Primary lyrics file. |
| cover | Cover art file. |

## Editing Notes

- Back up before editing.
- Keep paths relative to the feedpak.
- Do not rename files without updating the manifest.
- Validate after editing.

## Related Pages

- [What Is a feedpak?](index.md)
- [Validating feedpak Files](validation.md)

