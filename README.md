# MP3 Downloader

Simple Bash script to download and convert audio from YouTube to high-quality MP3 format using `yt-dlp`. This script supports direct downloads via URL as well as bulk/batch downloads using text files.

---

## Features

* **Automatic convert to MP3**
* **High quality audio**
* **Embed Metadata & Thumbnail**
* **Batch Download**

---

## Dependencies

Make sure your system (Linux / macOS / WSL) has the following dependencies installed:

1. **Bash Shell**
2. **yt-dlp** (Latest version recommended)
3. **ffmpeg** (Needed for audio, thumbnail, and metadata conversion)

### Dependency Installation (Ubuntu/Debian/Mint/Pop!_OS)
```bash
sudo apt update
sudo apt install ffmpeg yt-dlp -y
```

### (Arch/Manjaro/EndeavourOS/CachyOS)
```bash
sudo pacman -Syu
sudo pacman -S ffmpeg yt-dlp
```

### (Void)
```bash
sudo xbps-install -Su
sudo xbps-install ffmpeg yt-dlp
```

---

## Installation

```bash
git clone https://github.com/r4ymrch/mp3-downloader.git
cd mp3-downloader
chmod +x ./mp3-downloader
```

---

## Usage

### 1. Direct download from URL
```bash
./mp3-downloader -l "URL"
```

Also support multiple URL like this:
```bash
./mp3-downloader -l "URL_1" "URL_2" "URL_3"
```

---

### 2. Batch download

1. Create new file (example `lists.txt`) and fill it with a list of YouTube URLs (one URL per line):
   ```text
   URL_1
   URL_2
   URL...
   ```

2. Run the script with flag `-b` or `--batch`:
   ```bash
   ./mp3-downloader -b lists.txt
   ```

---

## License
Free to use and modify for personal needs.
