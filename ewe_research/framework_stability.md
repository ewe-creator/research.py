# Stability & Quality: The Backbone of Trust

To achieve a "Stable Version", your framework must rely on automated verification, not manual luck.

## 1. The Testing Pyramid

You cannot have a stable framework without a comprehensive test suite.

*   **Unit Tests**: 70% of tests. Fast, isolated.
*   **Integration Tests**: 20% of tests. Test plugin systems and DB connections.
*   **End-to-End (E2E) Tests**: 10% of tests. Real-world usage scenarios.

### Tooling
*   **Pytest**: The industry standard. Use fixtures heavily.
*   **Tox / Nox**: For testing against multiple Python versions (3.9, 3.10, 3.11, 3.12).

## 2. Automated Quality Assurance (CI/CD)

Never trust code that hasn't passed CI. Use **GitHub Actions**.

### Recommended Workflow (`.github/workflows/test.yml`)
1.  **Linting**: Run `ruff` (fastest linter) to catch syntax and style errors.
2.  **Type Checking**: Run `mypy --strict`.
3.  **Tests**: Run `pytest` across matrix of OS (Ubuntu, Windows, Mac) and Python versions.
4.  **Coverage**: Fail the build if coverage drops below 90%.

## 3. Strict Versioning (Stability)

Adhere rigorously to **Semantic Versioning (SemVer)**.
*   `MAJOR`: Breaking changes.
*   `MINOR`: New features, backwards compatible.
*   `PATCH`: Bug fixes only.

**Rule**: Never break user code in a MINOR or PATCH release. Use `DeprecationWarning` for at least two MINOR versions before removing an API.

## 4. Code Consistency Tools

Enforce consistency automatically.
*   **Ruff**: One tool to rule them all (imports, linting, formatting).
*   **Pre-commit hooks**: prevent bad code from even entering the repo.

```yaml
# .pre-commit-config.yaml
repos:
  - repo: https://github.com/astral-sh/ruff-pre-commit
    rev: v0.1.0
    hooks:
      - id: ruff
        args: [ --fix ]
      - id: ruff-format
```
