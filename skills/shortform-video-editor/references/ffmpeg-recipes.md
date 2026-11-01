# FFmpeg Recipes

Probe source:
```bash
ffprobe -v error -show_format -show_streams -of json input.mp4
```

Vertical scale and crop (center crop; inspect subject position first):
```bash
ffmpeg -i input.mp4 -vf "scale=1080:1920:force_original_aspect_ratio=increase,crop=1080:1920" -c:v libx264 -crf 20 -preset medium -pix_fmt yuv420p -c:a aac -b:a 192k -movflags +faststart output.mp4
```

Burn in an SRT subtitle file:
```bash
ffmpeg -i input.mp4 -vf "subtitles=captions.srt" -c:v libx264 -crf 19 -preset medium -c:a copy output_captioned.mp4
```

Extract a cover frame:
```bash
ffmpeg -ss 00:00:02 -i input.mp4 -frames:v 1 -q:v 2 cover.jpg
```

Create a review contact sheet (requires FFmpeg filters):
```bash
ffmpeg -i input.mp4 -vf "fps=1/3,scale=240:-1,tile=4x4" -frames:v 1 contact-sheet.jpg
```

These are starting recipes. Confirm FFmpeg filter availability, subtitle path escaping, source rotation, frame rate, and crop framing before production use.
