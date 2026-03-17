# Data Mining Project

Coursework repository for the CS4168 data mining project based on the Spotify tracks dataset in [data/tracks2026.csv](data/tracks2026.csv).

## Repository Layout

- `data/` stores the shared dataset used by the project.
- `notebooks/` stores exploratory and report-oriented notebooks.
- `requirements.txt` is the shared dependency list.
- `SETUP.md` contains the detailed environment setup steps.

## Quick Start

Use Python `3.12` if possible.

```powershell
py -3.12 -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
```

Then choose the Python .venv as the kernel in Jupyter or VS Code.

## Team Workflow

- Keep local virtual environments out of the repository.
- Update `requirements.txt` only when the project actually needs a new package.
- Keep raw or shared input data in `data/`.
- Keep generated outputs such as figures, models, and temporary exports out of Git.

