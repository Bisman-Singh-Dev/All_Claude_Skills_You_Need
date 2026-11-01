# Batch Automation Reference

## Safe batch pattern
```python
from pathlib import Path
import json

source_dir = Path("input")
output_dir = Path("output")
output_dir.mkdir(parents=True, exist_ok=True)

manifest = []
for src in sorted(source_dir.glob("*.jpg")):
    dst = output_dir / f"{src.stem}_edited.jpg"
    try:
        # Call a well-tested transform(src, dst) here.
        manifest.append({"source": str(src), "output": str(dst), "status": "planned"})
    except Exception as exc:
        manifest.append({"source": str(src), "output": str(dst), "status": "error", "error": str(exc)})

(output_dir / "manifest.json").write_text(
    json.dumps(manifest, indent=2), encoding="utf-8"
)
```

Add a `--dry-run` option for large jobs, never overwrite originals by default, and make a manifest with per-file success/failure details. For production workflows, record tool versions and transformation parameters.
