# TrainerHub media

Compressed MP4 copies of the exercise clips that [TrainerHub](https://swissystem7.github.io/TrainerHub/) plays.
The originals live in Google Drive, which stays the source of truth. This repo only serves fast copies.

- Path: `<folder>/<Drive file id>.mp4`
- Encoding: H.264 (main) + AAC, short side 360 px, `-movflags +faststart`
- Served from GitHub Pages first (`https://swissystem7.github.io/TrainerHub-media/...`), then from jsDelivr pinned to a tag
  (`https://cdn.jsdelivr.net/gh/Swissystem7/TrainerHub-media@<tag>/...`). TrainerHub falls back to the Drive player if both fail.
- New clips are added with `scripts/media_sync.py` in the TrainerHub repo. Its manifest is `videos/media-manifest.json`.
