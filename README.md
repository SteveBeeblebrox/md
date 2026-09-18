# `%md ...`
Write markdown in Jupyter code blocks that renders in the output and accumulates into a `README.md`.

## Usage
```python
exec(__import__('requests').get('https://raw.githubusercontent.com/SteveBeeblebrox/md/refs/heads/main/md').text)
```

```
%md # Header
%md Lorem Ipsum

# Interpolate values with {}
# Use double braces to escape
x = 2
%md x is {x}
```
