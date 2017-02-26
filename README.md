# Base16 for [prompt-toolkit](https://github.com/jonathanslenders/python-prompt-toolkit) (and [ipython](https://ipython.org/)!)

Clone this somewhere such that the directory `base16` is in (or is symlinked
from) your `PYTHONPATH`.

Then import your preferred theme using `importlib`:

```python
theme = importlib.import_module('base16.base16-default-dark')
```

Here is a complete example that configures ipython with `default-dark`:

```python
theme = importlib.import_module('base16.base16-default-dark')
c.TerminalInteractiveShell.highlighting_style = theme.Base16Style
c.TerminalInteractiveShell.highlighting_style_overrides = theme.overrides
```

That's it!
