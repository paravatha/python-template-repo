# python-template-repo

A minimal Python template to bootstrap new projects with a clean structure and modern tooling.

## What this repository provides

- Standard project layout (`src/`, `tests/`, `scripts/`, `notebooks/`)
- Dependency and environment management with `uv`
- Linting and formatting setup with `ruff` (v0.16+)
- Type-checking configuration with `pyright`
- Data validation with `pydantic` (v2.13+)
- Comprehensive testing framework with `pytest` (v9.1+)
- Jupyter notebook support with `ipykernel` (v7.3+) and `marimo` (v0.22+)

## Requirements

- Python `3.13.x`
- `uv` installed

## Quick start

```bash
# from repository root
uv python pin 3.13
uv sync
```

## Dependency Groups

The project uses organized dependency groups for different purposes:

- **`test`** - Testing framework (pytest, pytest-mock, pytest-asyncio, pytest-cov)
- **`lint`** - Code quality tools (ruff, ty)
- **`notebook`** - Jupyter and data science tools (ipython, ipykernel, marimo, nbstripout)
- **`build`** - Build and packaging tools (setuptools, prek)

Install specific groups with: `uv sync --group test --group lint`
Or install all groups: `uv sync --all-groups`

## Common commands

```bash
# run tests with coverage
uv run pytest --cov=src tests/

# lint
uv run ruff check .

# format
uv run ruff format .

# type checking
uv run pyright

# run tests
uv run pytest
```

## Project structure

```text
python-template-repo/
├── notebooks/
├── scripts/
├── src/
├── tests/
├── pyproject.toml
└── README.md
```

## Customization

- Update project metadata and dependencies in `pyproject.toml`.
- Add application code under `src/`.
- Add tests under `tests/`.
