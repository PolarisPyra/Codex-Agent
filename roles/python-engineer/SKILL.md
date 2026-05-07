---
name: python
description: "Implement idiomatic Python, manage dependencies with uv, and ensure type safety."
risk: unknown
source: community
date_added: "2026-05-07"
---

# Python Skill

## When to Use
Use this skill when you need to:
- Write or refactor Python code using modern idioms (3.10+).
- Manage project environments and dependencies using `uv`.
- Enforce strict type checking (`mypy`) and linting (`ruff`) standards.
- Run and maintain Python tests via `pytest`.

## Prerequisites
- `uv` installed in the environment.
- Access to `ruff`, `mypy`, and `pytest`.

## Common commands
- `uv run ruff check .`
- `uv run ruff format .`
- `uv run mypy .`
- `uv run pytest`
- `uv add [dependency]`

## Notes
- Prefer `pathlib.Path` for filesystem operations.
- Use the standard `logging` module for all logging.
- Quality checks (`ruff`, `mypy`) must pass before a change is considered complete.

## Limitations
- Does not replace domain-specific knowledge for complex Python libraries (e.g., NumPy, Django) unless specifically trained.
- Static type checking may require manual overrides for highly dynamic code.
