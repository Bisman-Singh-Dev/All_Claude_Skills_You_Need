# Rendering and Quality Control

## Video
- Verify dimensions, frame rate, duration, codec, pixel format, and audio streams with ffprobe.
- Inspect the full animation at normal playback speed.
- Check scene transitions and first/last frames.
- Watch for flicker, dropped frames, banding, and compression artifacts.

## Transparency
- Confirm the codec/container supports alpha.
- Check straight vs premultiplied alpha expectations.
- Inspect edges against both light and dark backgrounds.

## Still/vector assets
- Check SVG viewBox, clipping, font availability, and stroke scaling.
- Check raster resolution at final display size.
- Avoid accidental transparency flattening.
