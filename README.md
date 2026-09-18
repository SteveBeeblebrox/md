# `%md ...`
Write markdown in Jupyter code blocks that renders in the output and accumulates into a `README.md`.

To add `%md` to a notebook, run:
```python
exec(__import__('requests').get('https://raw.githubusercontent.com/SteveBeeblebrox/md/refs/heads/main/md').text)
```
Use `{expression}` to interpolate values from the enclosinscopesing
