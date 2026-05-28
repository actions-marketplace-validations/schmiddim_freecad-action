# Contributing

Contributions are welcome! Here's how to get started.

## Reporting Issues

Open an issue on [GitHub](https://github.com/schmiddim/freecad-action/issues) with:
- What you expected to happen
- What actually happened
- Steps to reproduce
- Your environment (OS, Docker version, FreeCAD version if relevant)

## Development Setup

```bash
# Clone the repo
git clone https://github.com/schmiddim/freecad-action.git
cd freecad-action

# Install Python dependencies
pip install -e ".[dev]"

# Build locally (requires Docker)
make build

# Build gallery only (no Docker needed)
python3 scripts/build_gallery.py

# Serve locally
make serve

# Validate YAML schemas
make validate
```

## Pull Requests

1. Fork the repo and create a branch from `master`
2. Use conventional commit messages (`feat:`, `fix:`, `refactor:`, `docs:`)
3. Test your changes locally with `make build` and `make validate`
4. Keep PRs focused -- one feature or fix per PR
5. Update documentation if your change affects user-facing behavior

## Project Structure

See the [README](README.md#project-structure) for an overview of the repository layout.

## Templates

HTML templates live in `scripts/templates/` and use Jinja2. CSS is in `scripts/templates/styles.css`. When editing templates:

- Run `python3 scripts/build_gallery.py` for fast iteration (no Docker needed)
- Use `make serve` to preview at `http://localhost:8000`
- All CSS goes in `styles.css` -- no inline styles in templates

## Releases

Releases are handled by maintainers via annotated git tags. The CI creates GitHub Releases and updates moving tags (`v2`, `v2.X`) automatically.
