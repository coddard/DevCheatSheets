Here's your **unified FFmpeg cheat sheet** with all sections combined into a single `.md` file:

---

# 🎞️ FFmpeg Cheat Sheet

**A colorful guide to FFmpeg commands for developers who love multimedia magic 🌟**

---

## 📚 Table of Contents

1. [🔄 Basic Conversion](#basic-conversion)
2. [🎨 High-Quality Encoding](#high-quality-encoding)
3. [✂️ Trimming & Cutting](#trimming--cutting)
4. [🧩 Merging & Combining](#merging--combining)
5. [⏱️ Timecode & Text Overlays](#timecode--text-overlays)
6. [🖼️ Image Watermarks](#image-watermarks)
7. [📝 Subtitle Management](#subtitle-management)
8. [📸 Frame Extraction](#frame-extraction)
9. [🌀 Deinterlacing & Filters](#deinterlacing--filters)
10. [📄 Metadata Manipulation](#metadata-manipulation)
11. [📡 Streaming & Downloading](#streaming--downloading)
12. [🔇 Audio Manipulation](#audio-manipulation)
13. 🧠 Pro Tips

---

## 🔁 Basic Conversion

**Convert between formats with ease!**

| Emoji | Command                                        | Description                     |
| ----- | ---------------------------------------------- | ------------------------------- |
| 🔄    | `ffmpeg -i in.mp4 out.avi`                     | Convert MP4 to AVI              |
| 🔄    | `ffmpeg -i in.mkv -c:v copy -c:a copy out.mp4` | Remux MKV to MP4 (no re-encode) |

---

## 🎨 High-Quality Encoding

**Control quality like a pro!**

| Emoji | Command                                           | Description                            |
| ----- | ------------------------------------------------- | -------------------------------------- |
| 🎨    | `ffmpeg -i in.mp4 -preset slower -crf 18 out.mp4` | Encode with CRF 18 (visually lossless) |

---

## ✂️ Trimming & Cutting

**Cut videos without breaking a sweat!**

| Emoji | Command                                                     | Description              |
| ----- | ----------------------------------------------------------- | ------------------------ |
| ✂️    | `ffmpeg -ss 00:01:30 -i in.mp4 -t 00:00:30 -c copy out.mp4` | Fast trim (no re-encode) |
| 🔁    | `ffmpeg -ss 00:01:30 -i in.mp4 -t 30 -c:v libx264 out.mp4`  | Trim with re-encode      |

---

## 🧩 Merging & Combining

**Combine media like a puzzle master!**

| Emoji | Command                                                          | Description                                  |
| ----- | ---------------------------------------------------------------- | -------------------------------------------- |
| 🧩    | `ffmpeg -i in0.mp4 -i in1.mp4 -map 0:v -map 1:a -c copy out.mp4` | Merge video/audio from two files             |
| 📋    | `ffmpeg -f concat -i list.txt -c copy out.mp4`                   | Concatenate videos (create `list.txt` first) |

---

## ⏱️ Timecode & Text Overlays

**Burn timecodes and add text watermarks!**

| Emoji | Command                                                                                                                                     | Description                    |
| ----- | ------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------ |
| 💬    | `ffmpeg -i in.mp4 -vf "drawtext=fontfile=arial.ttf:text='Hello':fontcolor=white:x=(w-text_w)/2:y=(h-text_h)/2" out.mp4`                     | Add centered text watermark    |
| 🪶    | `ffmpeg -i in.mp4 -vf "drawtext=fontfile=arial.ttf:text='Example':fontcolor=white:alpha=0.4:x=10:y=10" out.mp4`                             | Add transparent text overlay   |
| ⏰    | `ffmpeg -i in.mp4 -vf "drawtext=fontfile=arial.ttf:timecode='01\\:00\\:00\\:00':rate=25/1:fontcolor=yellow:x=(w-text_w)/2:y=h/1.2" out.mp4` | Burn timecode at bottom center |

---

## 🖼️ Image Watermarks

**Overlay logos or images on videos!**

| Emoji | Command                                                                             | Description                         |
| ----- | ----------------------------------------------------------------------------------- | ----------------------------------- |
| 🖼️    | `ffmpeg -i in.mp4 -i logo.png -filter_complex overlay=main_w-overlay_w-5:5 out.mp4` | Overlay image watermark (top-right) |

---

## 📝 Subtitle Management

**Add, burn, or embed subtitles!**

| Emoji | Command                                                      | Description                                          |
| ----- | ------------------------------------------------------------ | ---------------------------------------------------- |
| 📄    | `ffmpeg -i in.mp4 -i subs.srt -c copy -c:s mov_text out.mp4` | Embed SRT subtitles in MP4/MOV                       |
| 🧾    | `ffmpeg -i in.mp4 -vf "subtitles=subtitle.srt" out.mp4`      | Burn subtitles directly into video (requires libass) |

---

## 📸 Frame Extraction

**Turn videos into images (or vice versa)!**

| Emoji | Command                                                        | Description                |
| ----- | -------------------------------------------------------------- | -------------------------- |
| 📸    | `ffmpeg -i in.mp4 -vf fps=1 thumb%04d.jpg`                     | Extract 1 frame per second |
| 📷    | `ffmpeg -i in.mp4 -ss 00:00:10 -vframes 1 thumb.jpg`           | Extract a single frame     |
| 🎥    | `ffmpeg -r 1/5 -i img%03d.png -c:v libx264 -vf fps=25 out.mp4` | Create video from images   |

---

## 🌀 Deinterlacing & Filters

**Polish your video with filters!**

| Emoji | Command                                    | Description                          |
| ----- | ------------------------------------------ | ------------------------------------ |
| 🌀    | `ffmpeg -i in.mp4 -vf yadif out.mp4`       | Deinterlace video using yadif filter |
| 🔄    | `ffmpeg -i in.mov -vf transpose=1 out.mov` | Rotate 90° clockwise                 |

---

## 📄 Metadata Manipulation

**Tweak hidden video details!**

| Emoji | Command                                                                                    | Description                |
| ----- | ------------------------------------------------------------------------------------------ | -------------------------- |
| 📄    | `ffmpeg -i in.mp4 -map_metadata -1 -metadata title="My Title" -c:v copy -c:a copy out.mp4` | Remove metadata, set title |

---

## 📡 Streaming & Downloading

**Download and process streams!**

| Emoji | Command                                                                                 | Description                      |
| ----- | --------------------------------------------------------------------------------------- | -------------------------------- |
| 📡    | `ffmpeg -i path_to_playlist.m3u8 -c copy out.mp4`                                       | Download HLS stream              |
| 🔒    | `ffmpeg -protocol_whitelist "file,http,https,tcp,tls" -i playlist.m3u8 -c copy out.mp4` | Fix "Protocol not allowed" error |

---

## 🔇 Audio Manipulation

**Mute, boost, or silence audio!**

| Emoji | Command                                                             | Description              |
| ----- | ------------------------------------------------------------------- | ------------------------ |
| 🔇    | `ffmpeg -i in.mp4 -af "volume=enable='lte(t,90)':volume=0" out.mp4` | Silence first 90 seconds |
| 🔊    | `ffmpeg -i in.mp4 -af 'volume=0.5' out.mp4`                         | Boost audio volume (50%) |

---

## 🧠 Pro Tips

**Level up your FFmpeg game!**

- 🧹 **Clean output**: Add `-hide_banner` to hide FFmpeg version noise.
- 🚀 **Batch processing**:
  ```bash
  for file in *.mp4; do ffmpeg -i "$file" -preset slower "${file%.mp4}_crf18.mp4"; done
  ```
- 🧊 **Stream copy**: Use `-c copy` for instant cuts (no re-encode).
- 📊 **Debug errors**:
  ```bash
  ffmpeg -i input.mp4 -v error -f null - 2>error.log
  ```

---
