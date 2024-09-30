# KEH Documentation Structure
### Overview
This example repository highlights how KEH uses MkDocs for the documentation on each project. More information can be found on the [KEH's confluence page](https://confluence.ons.gov.uk/display/KEH/Code+Documentation).

### Setup

To get started clone the project using git, GitHub desktop or by downloading the zip file.

Once downloaded, if you don't have python3 installed please see [this](https://www.python.org/downloads/) to install.

### Installation
Alternatively, use [MkDocs installation instructions](https://www.mkdocs.org/getting-started/).

Install virtual env and poetry:
```bash
pip3 install virtualenv poetry
```

Initiate virtual environment:
```bash
python3 -m venv venv
```

Activate venv:
```bash
source venv/bin/activate
```

Install dependencies:
```bash
poetry install
```

Run MkDocs:
```bash
mkdocs serve
```

Edit the markdown files in docs.

### Deployment

Once you've finished editing the MkDocs, delete the `mkdocs_deployment` folder and run:

```bash
mkdocs build
```

and rename the `site` folder to `mkdocs_deployment`.

## Deploying to GitHub Pages
For more info, follow [MkDocs instructions](https://www.mkdocs.org/user-guide/deploying-your-docs/).

```bash
mkdocs gh-deploy
```

## Documentation
 
This project uses MkDocs for documentation which gets deployed to GitHub Pages at a repository level.
 
For more information about MkDocs, see the below documentation.
 
[Getting Started with MkDocs](https://www.mkdocs.org/getting-started/)
 
There is a guide to getting started on this repository's GitHub Pages site.