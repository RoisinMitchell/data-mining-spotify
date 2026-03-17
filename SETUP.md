# Project Setup

This project uses a root-level `requirements.txt` and a local virtual environment that is not committed to version control.

## Recommended Team Convention

- Keep the shared dependency list in `requirements.txt`.
- Each teammate creates their own local virtual environment.
- Do not treat `.venv/pyvenv.cfg` as a shared config file. It is machine-specific and points to one local Python installation.
- Do not commit `.venv/`, notebook checkpoints, cache files, generated figures, or model artifacts.

## Python Version

Use Python `3.12` if possible.

Reason:
- it is a stable target for data-science packages
- it is less likely to cause compatibility issues across teammates than a very new Python release

## Create the Environment

From the project root:

```powershell
py -3.12 -m venv .venv
```

Activate it on Windows PowerShell:

```powershell
.\\.venv\\Scripts\\Activate.ps1
```

Install dependencies:

```powershell
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
```

Then select the Python .venv inside Jupyter or VS Code for the notebooks.

## Updating Dependencies

Only add packages to `requirements.txt` when they are genuinely needed by the project.

When adding one:

1. Install it in your local environment.
2. Confirm the notebook or script actually uses it.
3. Add it to `requirements.txt`.
4. Let the team know to reinstall dependencies.

## Quick Start

```powershell
py -3.12 -m venv .venv
.\\.venv\\Scripts\\Activate.ps1
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
```
