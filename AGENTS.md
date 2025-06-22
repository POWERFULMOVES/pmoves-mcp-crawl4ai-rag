# Project Guidelines for Codex Agents

- Format Python code with `black` before committing.
- Run `pytest -q` after making changes. If tests fail because dependencies are missing, note this in the PR summary.
- Add any new Python dependencies to `pyproject.toml` and update `uv.lock` using `uv pip install`.
- Document configuration options and environment variables in `README.md` and `.env.example` when they change.
- Keep the working tree clean (`git status --short` should show no changes) before creating a pull request.

Additional Python packages are required to run the optional knowledge graph scripts and tests:
- pydantic_ai
- graphiti_core
- rich
Ensure these are installed before running pytest or the knowledge graph utilities.
