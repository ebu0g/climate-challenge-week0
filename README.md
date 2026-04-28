# Climate Challenge Week 0

This repository is set up as a lightweight Python workspace for climate-related exercises, notebooks, and scripts.

## Project Layout

The expected structure is:

```text
.
├── .vscode/
│   └── settings.json
├── .github/
│   └── workflows/
│       └── unittests.yml
├── .gitignore
├── requirements.txt
├── README.md
├── src/
├── notebooks/
│   ├── __init__.py
│   └── README.md
├── tests/
│   └── __init__.py
└── scripts/
    ├── __init__.py
    └── README.md
```

## Local Setup

1. Create and activate a virtual environment.

```bash
python -m venv venv
venv\\Scripts\\activate
```

1. Install the project dependencies.

```bash
pip install -r requirements.txt
```

1. Run the test suite.

```bash
pytest
```

## Development Notes

- Use `src/` for reusable code.
- Use `notebooks/` for exploratory analysis.
- Use `scripts/` for one-off or repeatable command-line helpers.
- Keep tests in `tests/` and run them locally before pushing changes.

## CI

GitHub Actions runs the test suite on pushes and pull requests targeting `main`.