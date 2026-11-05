# Video Player — Two Languages

A single-file, offline video player for language learners. Load a video and two subtitle files (for example English and Persian). Only the English subtitle is shown. When you don't understand a sentence, press `P` to reveal the translation for that sentence only.

Everything runs locally in your browser. Nothing is uploaded anywhere.

## Usage

1. Open `index.html` in your browser (double-click it, or use the GitHub Pages link if enabled).
2. Choose your video file.
3. Choose the English subtitle and the Persian subtitle.
4. Watch. Press `P` whenever you need the translation.

## Keyboard shortcuts

Shortcuts use physical keys, so they also work with a Persian keyboard layout.

| Key | Action |
| --- | --- |
| `Space` | Play / pause (only this, nothing else) |
| `P` | Show / hide the Persian subtitle for the current sentence |
| `R` | Repeat the current sentence |
| `A` / `D` | Previous / next sentence |
| `Z` / `X` | Slower / faster playback (0.5× – 2×) |
| `T` | Toggle auto-pause at the end of each sentence |
| `[` / `]` | Move Persian subtitle earlier / later (0.5 s, hold `Shift` for 0.1 s) |
| `-` / `=` | Move English subtitle earlier / later (0.5 s, hold `Shift` for 0.1 s) |
| `←` / `→` | Seek 5 seconds back / forward |
| `F` | Toggle fullscreen (also the on-screen button or a double-click on the video) |

The Persian subtitle is hidden automatically when the next sentence starts.

## Subtitle synchronization

If the two subtitle files don't line up, click **Auto-sync Persian**. The player compares when speech occurs in both files, finds the time shift, and also corrects slow drift caused by different frame rates. Use `[` / `]` for manual fine-tuning, or **Reset sync** to start over.

If the English subtitle itself is early or late relative to the video, use `-` / `=`.

## Features

- SRT and VTT subtitle support
- UTF-8 and Windows-1256 (Persian) encodings detected automatically
- Right-to-left rendering for the Persian subtitle
- Persian lines are matched to English sentences by time overlap, so different line splitting is handled
- Click any English word to open its translation (needs an internet connection; can be turned off)
- Subtitles stay visible in fullscreen
- No installation, no dependencies, no network access (except the optional word lookup)

## Notes

- Playback depends on your browser's codecs. MP4 (H.264) and WebM work best; some MKV files may not play.

## License

Licensed under the [Polyform Strict License 1.0.0](LICENSE). Noncommercial use is permitted; distribution and derivative works are not.
