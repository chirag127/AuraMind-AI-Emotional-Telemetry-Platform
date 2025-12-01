# Pull Request Template

**Please follow these guidelines when submitting a Pull Request:**

1.  **Commit Message Style:**
    *   Use Conventional Commits: `<type>(<scope>): <subject>

        <body>

        <footer>`
    *   **Types:** `feat`, `fix`, `chore`, `docs`, `style`, `refactor`, `perf`, `test`.
    *   **Scope:** Optional, specifying the part of the codebase affected (e.g., `api`, `extension`, `ui`).
    *   **Subject:** Concise, imperative mood, capitalized (e.g., `feat: Implement user authentication`).
    *   **Body:** Explain *what* and *why*, not *how*.
    *   **Footer:** For breaking changes (`BREAKING CHANGE: ...`) or closing issues (`Closes #123`).

2.  **Code Quality:**
    *   **Linting & Formatting:** Ensure code passes `ruff check` and `ruff format` without errors. Run `uv run Ruff-check .` and `uv run Ruff-format .` locally before committing.
    *   **Type Hinting:** All functions, methods, and relevant variables must have strict type hints.
    *   **Testing:** All new features must include comprehensive unit tests. All fixes must include tests that reproduce the bug. Ensure all tests pass (`pytest`). Run `uv run pytest` locally.
    *   **Architecture:** Adhere to Hexagonal Architecture principles. Ensure clear separation between domain, adapters, and ports.

3.  **Testing & Verification:**
    *   [ ] **Local Tests Pass:** All `pytest` suites are passing.
    *   [ ] **Linting & Formatting Applied:** Code adheres to `ruff` standards.
    *   [ ] **New Functionality Covered by Tests:** New code paths have corresponding unit/integration tests.
    *   [ ] **Bug Fixes Verified:** Tests confirm the bug is resolved.

4.  **Description:**
    *   **What does this PR do?** Briefly summarize the changes.
    *   **Why is this PR needed?** Explain the problem it solves or the feature it adds.
    *   **How was it implemented?** Highlight key architectural decisions or implementation details.
    *   **Screenshots/GIFs:** Include visual aids for UI changes if applicable.
    *   **Related Issues:** Link to any relevant issues (e.g., `Closes #123`, `Fixes #456`).

5.  **Reviewer Checklist:**
    *   [ ] The PR is small and focused.
    *   [ ] The code is clear, readable, and well-documented.
    *   [ ] The changes align with the project's goals and architecture.
    *   [ ] Potential side effects or regressions have been considered.
    *   [ ] The PR includes appropriate tests.

---