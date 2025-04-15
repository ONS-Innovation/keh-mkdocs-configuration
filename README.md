# KEH Documentation Structure
## Overview
This example repository highlights how KEH uses MkDocs for the documentation on each project. More information can be found on the [KEH's confluence page](https://confluence.ons.gov.uk/pages/viewpage.action?pageId=225098833).

## Prerequisites

To install and run MkDocs, you are required to have Python's package manager, PIP, installed. See [Python's website](https://www.python.org/) for more information. 

## Getting MkDocs Setup

In order to build an MkDocs deployment or serve the documentation locally, we need to install MkDocs and its dependencies.

1. Navigate into the project's root directory.

2. Create a virtual environment and activate it.

    ```bash
    python3 -m venv venv
    source venv/bin/activate
    ```

2. Install MkDocs and its dependencies.

    ```bash
    pip install -r mkdocs_requirements.txt
    ```

3. You can now use MkDocs. To see a list of commands run the following:

    ```bash
    mkdocs --help
    ```

## Deployment

Once you've finished editing the documentation, you can run it locally to see how it looks.

To run the documentation locally, run the following command:

```bash
mkdocs serve
```

If you're happy with the documentation, you can deploy the documentation to GitHub Pages. To do this, run the following command:

```bash
mkdocs gh-deploy
```

This will build the documentation and deploy it to the `gh-pages` branch of your repository. The documentation will be available at `https://ONS-Innovation.github.io/<repository-name>/`.

## Housekeeping

Your repository should include the following in your README.md file:
```
## Documentation
 
This project uses MkDocs for documentation which gets deployed to GitHub Pages at a repository level.
 
For more information about MkDocs, see the below documentation.
 
[Getting Started with MkDocs](https://www.mkdocs.org/getting-started/)
 
There is a guide to getting started on this repository's GitHub Pages site.
```

## Extra Information

For more information on how to use and implement this setup into other projects, please see [KEH's confluence page](https://confluence.ons.gov.uk/pages/viewpage.action?pageId=225098833).