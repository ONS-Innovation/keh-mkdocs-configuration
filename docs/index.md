# KEH Documentation Example

## Overview

This is an example website using KEH's documentation setup. More information, such as how to use this setup in your own projects, can be found at [KEH's confluence page](https://confluence.ons.gov.uk/display/KEH/Code+Documentation).

## Material for MkDocs

KEH documentation sites use [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/). This includes theming for the site and a range of useful features which extends markdown capabilities.

### Adding Material Features

All addition features provided by Material can be found [here](https://squidfunk.github.io/mkdocs-material/reference/).

If you find an addition feature you require, add it to `mkdocs.yml`.

For example, if you wanted to include [Admonitions](https://squidfunk.github.io/mkdocs-material/reference/admonitions/) within your website, you would need to add the following to `mkdocs.yml`:

```yml
markdown_extensions:
  - admonition
  - pymdownx.details
  - pymdownx.superfences
```

**Note:** Some extensions may already be added to `mkdocs.yml`. Make sure to check the existing extensions **before** adding new ones.

### Example - Material Diagrams using Mermaid.js

When using the `mkdocs.yml` provided by this repository, it comes with some extensions by default. One of these extensions is [diagrams using Mermaid.js](https://squidfunk.github.io/mkdocs-material/reference/diagrams/). This extension allows you to define a range of useful diagrams in markdown.

#### Example Flowchart

An example of this extension is the flowchart below.

**markdown definition:**

````markdown
``` mermaid
graph LR
  A[Start] --> B{Error?};
  B -->|Yes| C[Hmm...];
  C --> D[Debug];
  D --> B;
  B ---->|No| E[Yay!];
```
````

**diagram output:**

``` mermaid
graph LR
  A[Start] --> B{Error?};
  B -->|Yes| C[Hmm...];
  C --> D[Debug];
  D --> B;
  B ---->|No| E[Yay!];
```

## Mkdocstrings

Mkdocstrings is plugin included in KEH's setup. This plugin generates code documentation based of docstrings written in code. For more information, read their [documentation](https://mkdocstrings.github.io/). If using the `mkdocs.yml` file provided by this repository, mkdocstrings will automatically work with Python. The following config has been added to `mkdocs.yml`:

```yml
plugins:
  - mkdocstrings:
      default_handler: python
```

Mkdocstrings does support other languages. Please see their [usage guide](https://mkdocstrings.github.io/usage/) for more information.

### Example - GitHub API Toolkit

This functionality has been used within KEH's GitHub API Toolkit (written in Python).

**markdown definition:**

```markdown
# `github_graphql_interface()`

::: github_api_toolkit.github_graphql_interface
```

**output:**

[github_graphql_interface :link:](https://ons-innovation.github.io/github-api-package/reference/github_graphql_interface/)

## Additional MkDocs Functionality

Feel free to add other `markdown_extensions` or `plugins` to this MkDocs setup. If you think a plugin/extension is of great use and applicable to a large number of projects, please raise a GitHub Issue or Pull Request to get it added.