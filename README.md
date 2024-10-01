# KEH Documentation Structure
### Overview
This example repository highlights how KEH uses MkDocs for the documentation on each project. More information can be found on the [KEH's confluence page](https://confluence.ons.gov.uk/display/KEH/Code+Documentation).

### Getting MkDocs Setup
Alternatively, use [MkDocs installation instructions](https://www.mkdocs.org/getting-started/).

In order to build an MkDocs deployment or serve the documentation locally, we need to install MkDocs and its dependencies.

1. Navigate into the project's root directory.

2. Install MkDocs and its dependencies.

    ```bash
    pip install -r mkdocs_requirements.txt
    ```

3. You can now use MkDocs. To see a list of commands run the following:

    ```bash
    mkdocs --help
    ```

**Please Note:** Python's package manager, PIP, is required to install MkDocs. Please make sure you have Python installed beforehand.


### Deployment

Once you've finished editing the MkDocs, delete the `mkdocs_deployment` folder and run:

```bash
mkdocs build
```

and rename the `site` folder to `mkdocs_deployment`.

Make sure to include `.github/workflows/deploy_mkdocs.yml` in your repository so when your code is merged or committed to main, it redeploys the GitHub pages.

## Deploying to GitHub Pages
Make sure the `.github/workflows/deploy_mkdocs.yml` is in your root folder and commit to main, the GitHub action should deploy your MkDocs to GitHub Pages.

Your repository should include this in your README.md file:
```
## Documentation
 
This project uses MkDocs for documentation which gets deployed to GitHub Pages at a repository level.
 
For more information about MkDocs, see the below documentation.
 
[Getting Started with MkDocs](https://www.mkdocs.org/getting-started/)
 
There is a guide to getting started on this repository's GitHub Pages site.
```