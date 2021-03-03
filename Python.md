# Python

## PIL save to memory
```python
import io

im: PIL.Image.Image = PIL.open("data.jpg")

buf = io.BytesIO()
im.save(buf, format="PNG")
im_bytes = buf.getvalue()
```

## 判断Python版本 Check Python version
```python
import sys

sys.version_info[:2] >= (3, 6)
```