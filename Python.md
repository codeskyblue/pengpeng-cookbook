# Python

## 常用环境变量
```
PYTHONIOENCODING=utf-8  # 强制编码
PYTHONUNBUFFERED=1  # 关闭缓存, 等价于-u
```

更多参考: https://docs.python.org/3/using/cmdline.html

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
