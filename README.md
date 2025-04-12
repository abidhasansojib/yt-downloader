# yt-downloader

A lightweight YouTube audio/video downloader for Termux using `yt-dlp`.

This CLI tool allows you to quickly download audio (MP3) or full-quality video directly into your phone's `/sdcard/yt` folder — with storage permission and directory handling done automatically.

---

## Features

- Downloads **audio** or **video** in best quality
- Automatically requests **Termux storage permission** (if needed)
- Creates `/sdcard/yt` directory if it doesn't exist
- Outputs files using the video title
- Built for Android Termux users

---

## Installation (Termux)

Run this one-liner in your Termux terminal:

```bash
pkg install git -y && \
git clone https://github.com/abidhasansojib/yt-downloader && \
cd yt-downloader && \
mv yt $PREFIX/bin && \
chmod +x $PREFIX/bin/*

```

## How to Use

Once the `yt` command is installed, you can use it to download either audio or video by passing a YouTube URL with the appropriate flag:

### Audio Download

```bash
yt -a <YouTube_URL>

```

Downloads the best quality audio as an .mp3 file.

##Video Download


```bash
yt -v <YouTube_URL>

```

Downloads the best quality video (with merged audio) as an .mp4 file.

	
