## Installation

```bash
pip install \
    mkdocs \
    mkdocs-material \
    mkdocs-minify-plugin \
    mkdocs-autolinks-plugin \
    pymdown-extensions \
    mkdocs-git-revision-date-localized-plugin
```

## Create

Create the `docs` repository.

```sh
mkdocs new docs
```

## Configuration

```yaml title="mkdocs.yml"
site_name: Mkdocs Example
site_url: https://example.com
nav:
  - Home: index.md
  - Markdown: markdown.md
  - About: about.md

plugins:
  - search
  - autolinks
  - minify:
      minify_html: true
  - git-revision-date-localized:
      type: timeago

# theme: readthedocs
theme:
  name: material
  palette:
    # Palette toggle for light mode
    - scheme: defaultmk
      toggle:
        icon: material/brightness-7
        name: Switch to dark mode
    # Palette toggle for dark mode
    - scheme: slate
      toggle:
        icon: material/brightness-4
        name: Switch to light mode
  features:
    - content.code.copy

markdown_extensions:
  - admonition
  - meta
  - toc:
      permalink: true
      baselevel: 2
  - pymdownx.highlight:
      anchor_linenums: true
      line_spans: __span
      pygments_lang_class: true
  - pymdownx.inlinehilite
  - pymdownx.snippets
  - pymdownx.superfences

```

## Run

```sh
mkdocs serve
mkdocs build
```
