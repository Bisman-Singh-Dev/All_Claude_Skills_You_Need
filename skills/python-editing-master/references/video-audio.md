# Video and Audio Reference

## Inspect with ffprobe
```bash
ffprobe -v error -show_format -show_streams -of json input.mp4
```

## Trim without re-encoding (only when stream boundaries and codecs permit)
```bash
ffmpeg -ss 00:00:05 -i input.mp4 -t 00:00:20 -c copy output.mp4
```

## High-quality H.264 export
```bash
ffmpeg -i input.mp4 -c:v libx264 -preset medium -crf 18 -c:a aac -b:a 192k output.mp4
```

## Extract a representative frame
```bash
ffmpeg -ss 00:00:03 -i input.mp4 -frames:v 1 preview.png
```

Always inspect the output with ffprobe and view frames at the beginning, middle, and end. Check audio synchronization and preserve subtitles or extra streams when required.
