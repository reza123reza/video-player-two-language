# Video Player — Two Languages

A single-file, offline video player for language learners. Load a video and two subtitle files (for example English and Persian). Only the English subtitle is shown. When you don't understand a sentence, press `P` to reveal the translation for that sentence only.

Everything runs locally in your browser. Nothing is uploaded anywhere.

## Usage

1. Open `index.html` in your browser (double-click it, or use the GitHub Pages link if enabled).
2. Choose your video file.
3. Choose the primary subtitle (e.g. English) and the secondary subtitle (e.g. Persian).
4. Watch. Press `P` whenever you need the translation.

## Keyboard shortcuts

| Key | Action |
| --- | --- |
| `Space` | Play / pause (only this, nothing else) |
| `P` | Show the secondary (Persian) subtitle for the current sentence |
| `←` / `→` | Seek 5 seconds back / forward |
| `F` | Toggle fullscreen (also the on-screen button or a double-click on the video) |

The secondary subtitle is hidden automatically when the next sentence starts.

## Features

- SRT and VTT subtitle support
- UTF-8 and Windows-1256 (Persian) encodings detected automatically
- Right-to-left rendering for the Persian subtitle
- Secondary subtitle is matched by time overlap, so the two files do not need identical timing
- No installation, no dependencies, no network access

## Notes

- Playback depends on your browser's codecs. MP4 (H.264) and WebM work best; some MKV files may not play.

## License

Licensed under the [Polyform Strict License 1.0.0](LICENSE). Noncommercial use is permitted; distribution and derivative works are not.
