# python-template-repo

A minimal Python template to bootstrap new projects with a clean structure and modern tooling.

## What this repository provides

- Standard project layout (`src/`, `tests/`, `scripts/`, `notebooks/`)
- Dependency and environment management with `uv`
- Linting and formatting setup with `ruff`
- Type-checking configuration with `pyright`

## Requirements

- Python `3.13.x`
- `uv` installed

## Quick start

```bash
# from repository root
uv python pin 3.13
uv sync
```

## Common commands

```bash
# run tests
uv run pytest

# lint
uv run ruff check .

# format
uv run ruff format .
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
