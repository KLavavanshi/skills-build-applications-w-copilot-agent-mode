# OctoFit Tracker App

This repository contains the scaffold for the OctoFit Tracker App.

## Project structure

- README.md
- requirements.txt
- .gitignore
- src/octofit/
  - __init__.py
  - main.py
- scripts/
  - create_venv.sh
- .github/workflows/ci.yml

## Python virtual environment and installation

1. Create a virtual environment (Unix/macOS):

   python3 -m venv .venv
   source .venv/bin/activate

   On Windows (PowerShell):

   python -m venv .venv
   .\.venv\Scripts\Activate.ps1

2. Upgrade pip and install requirements:

   python -m pip install --upgrade pip
   pip install -r requirements.txt

3. Run the app (development):

   uvicorn octofit.main:app --reload --host 127.0.0.1 --port 8000

## Notes

- A helper script is provided at scripts/create_venv.sh to create the venv and install the requirements on Unix-like systems.
- The repository includes a GitHub Actions workflow that sets up Python and installs requirements on push to build-octofit-app.
