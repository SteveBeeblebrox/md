# `%md ...`
Write markdown in Jupyter code blocks that renders in the output and accumulates into a `README.md`.

To get started, make a new notebook cell and run ```python
exec(__import__('requests').get('https://raw.githubusercontent.com/SteveBeeblebrox/md/refs/heads/main/md').text)
```
