# CONTRIBUTING GUIDELINES

Welcome to **AuraMind-AI-Emotional-Telemetry-Platform**! We appreciate your interest in contributing to this project. Our goal is to foster a collaborative environment where high-quality, well-architected code is paramount.

## 1. CODE OF CONDUCT

All contributors are expected to adhere to the [Contributor Covenant Code of Conduct](https://www.contributor-covenant.org/version/2/1/0/CODE_OF_CONDUCT.html). Please review it to understand our expectations for respectful and inclusive participation.

## 2. HOW TO CONTRIBUTE

We welcome contributions in the form of bug reports, feature requests, documentation improvements, and code contributions.

### 2.1. Reporting Bugs

If you find a bug, please report it via GitHub Issues. Before reporting, please:

1.  **Search existing issues:** Check if the bug has already been reported.
2.  **Provide detailed information:** Include:
    *   A clear, descriptive title.
    *   The environment (browser, OS, Node.js version, etc.).
    *   Steps to reproduce the bug.
    *   Expected behavior vs. actual behavior.
    *   Screenshots or console logs, if applicable.

### 2.2. Suggesting Enhancements & Features

Feature requests are also handled through GitHub Issues. Please structure your request with:

1.  A clear title summarizing the proposed feature.
2.  A detailed description of the feature and its benefits.
3.  Any potential use cases or scenarios it would address.
4.  Mockups or wireframes, if helpful.

### 2.3. Contributing Code

For code contributions, please follow these steps:

1.  **Fork the repository:** Create your own fork of the `AuraMind-AI-Emotional-Telemetry-Platform` repository.
2.  **Clone your fork:** `git clone https://github.com/<your-username>/AuraMind-AI-Emotional-Telemetry-Platform.git`
3.  **Set up upstream remote:** `git remote add upstream https://github.com/Apex-Labs/AuraMind-AI-Emotional-Telemetry-Platform.git`
4.  **Create a new branch:** `git checkout -b <branch-name>` (e.g., `feat/add-new-visualization`, `fix/resolve-memory-leak`). Use descriptive names.
5.  **Make your changes:** Adhere to the project's coding standards and architectural principles.
6.  **Test your changes:** Ensure all tests pass and ideally add new tests for your changes.
7.  **Lint and format:** Run `npm run lint` and `npm run format` (or relevant commands for the JS/TS stack).
8.  **Commit your changes:** Use [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) format (e.g., `feat: Implement new sentiment analysis model`).
9.  **Push to your fork:** `git push origin <branch-name>`
10. **Open a Pull Request (PR):** From your fork, open a PR against the `main` branch of the original `Apex-Labs/AuraMind-AI-Emotional-Telemetry-Platform` repository.

## 3. DEVELOPMENT WORKFLOW & STANDARDS

We enforce rigorous standards to ensure code quality, maintainability, and performance. All contributions must align with these principles:

*   **Apex Toolchain:** This project uses the **TypeScript 6.x (Strict), Vite 7, Tauri v2.x, WXT** stack with **Biome** for linting/formatting and **Vitest/Playwright** for testing.
*   **Architecture:** Feature-Sliced Design (FSD) and modularity are key. Code should be organized logically within `src/features/` or `src/entities/`.
*   **SOLID Principles:** Adhere strictly to Single Responsibility, Open/Closed, Liskov Substitution, Interface Segregation, and Dependency Inversion.
*   **Clean Code:** Write self-documenting code. Avoid magic numbers, use semantic naming, and employ guard clauses for early returns.
*   **Testing:** **100% test coverage is mandatory**. Every source file must have a corresponding test file in the `tests/` directory. Tests must be FAST, ISOLATED, and REPEATABLE.
*   **Security:** Follow the DevSecOps Protocol. Sanitize ALL inputs (OWASP Top 10 2025), use secure defaults, and ensure data privacy.
*   **Performance:** Optimize for efficiency. Ensure low INP (<200ms) and utilize lazy loading and efficient algorithms.
*   **CI/CD:** All PRs are automatically linted and tested. Ensure your changes pass all CI checks before submitting.

## 4. PULL REQUESTS (PRs)

*   **Target Branch:** All PRs should target the `main` branch.
*   **Description:** Use the provided PR template to detail your changes.
*   **Reviews:** All PRs require at least one approval from a core maintainer before merging.
*   **Squash and Merge:** We generally use squash and merge to maintain a clean Git history.

## 5. SUPPORTING THE PROJECT

*   **Documentation:** Clear and concise documentation is crucial. Help us improve it!
*   **Feedback:** Provide constructive feedback on existing issues and features.
*   **Star ⭐ This Repo:** If you find AuraMind valuable, please consider starring the repository on GitHub!

We look forward to your contributions!
