# Image Editing Reference

## Recommended pipeline
1. Load with Pillow and apply EXIF transpose.
2. Inspect mode, dimensions, ICC profile, alpha, and metadata.
3. Convert to an appropriate working mode; retain high bit depth where needed.
4. Apply edits with masks and separate intermediate layers where possible.
5. Composite in a deliberate order.
6. Convert to target color mode/profile and export once.
7. Reopen output and verify dimensions, mode, alpha, and file size.

## Example: safe resize
```python
from pathlib import Path
from PIL import Image, ImageOps

src = Path("input.jpg")
dst = Path("output/resized.jpg")
dst.parent.mkdir(parents=True, exist_ok=True)

with Image.open(src) as im:
    im = ImageOps.exif_transpose(im)
    im.thumbnail((2000, 2000), Image.Resampling.LANCZOS)
    if im.mode not in ("RGB", "L"):
        im = im.convert("RGB")
    im.save(dst, quality=94, optimize=True)

with Image.open(dst) as check:
    check.verify()
```

## Example: masked composite
```python
from PIL import Image

background = Image.open("background.jpg").convert("RGBA")
foreground = Image.open("subject.png").convert("RGBA")
mask = foreground.getchannel("A")
foreground = foreground.resize(background.size)
mask = mask.resize(background.size)
background.alpha_composite(Image.composite(foreground, Image.new("RGBA", foreground.size), mask))
background.save("composite.png")
```

For realistic composites, match scale, perspective, light direction, color temperature, edge softness, grain, and contact shadows. The example is only a structural starting point; it does not automatically create a realistic composite.
