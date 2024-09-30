# KEH Documentation Structure
This example repository highlights how KEH uses MkDocs for the documentation on each project.

To get started clone the project using git, GitHub desktop or by downloading the zip file.

Once downloaded, if you don't have python3 installed please see [this](https://www.python.org/downloads/) to install.

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

Edit the markdown files in docs (`docs/<file>.md`).