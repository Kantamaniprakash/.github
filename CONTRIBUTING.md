# Contributing

Thanks for your interest! These are primarily personal / portfolio projects, but
issues and pull requests are welcome.

## Getting started

1. **Fork** the repository and clone your fork.
2. Create a virtual environment and install dependencies:
   ```bash
   python -m venv .venv
   source .venv/bin/activate          # Windows: .venv\Scripts\activate
   pip install -r requirements.txt    # or: pip install -e ".[dev]"
   ```
3. Install the pre-commit hooks (where the repo provides a config):
   ```bash
   pip install pre-commit
   pre-commit install
   ```

## Making changes

- Create a topic branch: `git checkout -b feat/short-description`.
- Keep commits small and use clear, imperative messages
  (e.g. `Add walk-forward backtest`, not `update`).
- Run the checks locally before pushing:
  ```bash
  ruff check .          # lint
  ruff format .         # format
  pytest -q             # tests
  ```
- Open a pull request against the default branch. CI must pass before merge.

## Reporting bugs & requesting features

Open an issue describing the problem or proposal, including reproduction steps and
your environment where relevant.

## Security

Please **do not** file public issues for security problems — see
[SECURITY.md](SECURITY.md) for private reporting.
