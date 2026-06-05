# stupiyd
stupiyd

## Setup

To initialise the virtual environment and install dependencies, run:

```bash
source init.sh
```

**Note:** Use `source init.sh` (or `. init.sh`) rather than `sh init.sh` or `./init.sh`. Running it without `source` will install dependencies correctly, but the virtual environment activation won't persist in your terminal session.

To reactivate the virtual environment in a new terminal:

```bash
source .venv/bin/activate
```

## Pre-commit Hooks

The init script automatically installs pre-commit hooks that run on every commit:

- **Ruff** — lints (with auto-fix) and formats Python files
- **nbstripout** — strips output from Jupyter notebooks to keep diffs clean

To run the hooks manually against all files:

```bash
pre-commit run --all-files
```
