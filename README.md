# PanelPilot Documentation

Source for the [PanelPilot](https://github.com/) Blender addon documentation, built with Sphinx, MyST, and the Furo theme.

## Build locally

```bash
pip install -r requirements.txt
sphinx-build -b html docs docs/_build/html
```

The output is written to `docs/_build/html/index.html`.

## Publish on Read the Docs

1. Push this repository to GitHub.
2. Import the project on [Read the Docs](https://readthedocs.org/).
3. Read the Docs picks up `.readthedocs.yaml` automatically and builds the site.
