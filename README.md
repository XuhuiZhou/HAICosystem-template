![TITLE](figs/title.png)
# HAICosystem-demo

[![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)](https://www.python.org/downloads/release/python-3109/)
[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://pre-commit.com/)
[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
[![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)


## Get started

This package supports Python 3.11 and above. We recommend using a virtual environment to install this package, e.g.,

```
conda create -n haicosystem-demo python=3.11; conda activate haicosystem-demo;  curl -sSL https://install.python-poetry.org | python3
poetry install
```


## Usage
xxx


## Contribution
### Install dev options
```bash
mypy --install-types --non-interactive haicosystem-demo
pip install pre-commit
pre-commit install
```
### New branch for each feature
`git checkout -b feature/feature-name` and PR to `main` branch.
### Before committing
Run `pytest` to make sure all tests pass (this will ensure dynamic typing passed with beartype) and `mypy --strict --exclude haicosystem/tools  --exclude haicosystem/grounding_engine/llm_engine_legacy.py .` to check static typing.
(You can also run `pre-commit run --all-files` to run all checks)
### Check github action result
Check the github action result to make sure all tests pass. If not, fix the errors and push again.