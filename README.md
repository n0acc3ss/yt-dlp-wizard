# yt-dlp Command Wizard

An interactive, browser-based command builder for [yt-dlp](https://github.com/yt-dlp/yt-dlp). Configure every option through a visual UI and get a ready-to-paste terminal command — no manual flag-hunting required.

**[→ Open the Wizard](https://n0acc3ss.github.io/yt-dlp-wizard/)**

---

## Features

**Download modes**
- **Auto Best** — grabs the best pre-muxed format, no ffmpeg needed
- **Video + Audio** — separate stream merge with full codec and resolution control (H.264, H.265, VP9, AV1 / AAC, Opus, MP3)
- **Audio Only** — extracts to mp3, m4a, flac, wav, opus, aac, or alac with quality/bitrate control

**Output control**
- Save path with folder picker
- Filename templates (Title, Uploader, Date, Playlist index, custom `%(field)s` syntax, or a fixed name)

**Subtitles & Metadata**
- Manual or auto-generated subtitles, per-language, per-format
- Embed thumbnail, metadata, and subtitles into the container

**SponsorBlock**
- Mark or remove sponsor, intro, and outro segments by category

**Cookies & Auth**
- Pull cookies directly from Chrome, Firefox, Edge, Brave, and others
- Or point to a Netscape-format `cookies.txt` file

**Network**
- Rate limit, concurrent fragment count, proxy

**Flags** — simulate/dry-run, verbose, ignore errors, no-overwrites, restrict filenames, list formats

**Quick Presets** — 1080p MP4, MP3 Audio, 720p WebM, FLAC, Playlist download, Dry Run (desktop only)

---

## Usage

1. Open the wizard in a browser
2. Configure your options
3. Click **Copy Command**
4. Paste into a terminal where yt-dlp is installed

No installation, no server, no dependencies — runs entirely in the browser.

---

## Prerequisites

The wizard builds the command; you still need yt-dlp (and ffmpeg for merge mode) installed locally.

```bash
# Install yt-dlp
pip install -U yt-dlp

# Install ffmpeg (required for Video + Audio merge mode)
sudo apt install ffmpeg        # Debian/Ubuntu
brew install ffmpeg            # macOS
```

---

## Local Development

Just open `index.html` in a browser — it's a single self-contained file with no build step.

---

## License

[MIT](LICENSE)
