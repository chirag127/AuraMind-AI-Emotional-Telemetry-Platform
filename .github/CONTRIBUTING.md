# Contributing to AuraMind-AI-Emotional-Telemetry-Platform

Thank you for your interest in contributing to AuraMind-AI-Emotional-Telemetry-Platform! We aim for a high-velocity, zero-defect development process, adhering to FAANG-level standards and the wisdom of "Managing the Unmanageable." By contributing, you agree to uphold these standards and the project's philosophy: "Zero-Defect, High-Velocity, Future-Proof."

## 1. Code of Conduct

This project adheres to a Contributor Covenant Code of Conduct. Please review the [CODE_OF_CONDUCT.md](https://github.com/chirag127/AuraMind-AI-Emotional-Telemetry-Platform/blob/main/CODE_OF_CONDUCT.md) file for details.

## 2. Prerequisites

Before you can contribute, ensure you have the following set up:

*   **Node.js:** Version 20+ (Required for both extension and API development).
*   **npm/yarn/pnpm:** A package manager.
*   **Git:** Latest stable version.
*   **IDE:** VS Code with TypeScript and Prettier extensions recommended.

## 3. Getting Started

1.  **Fork the Repository:** Create your own fork of `chirag127/AuraMind-AI-Emotional-Telemetry-Platform`.
2.  **Clone Your Fork:** `git clone git@github.com:chirag127/AuraMind-AI-Emotional-Telemetry-Platform.git`
3.  **Navigate to Project:** `cd AuraMind-AI-Emotional-Telemetry-Platform`
4.  **Install Dependencies:**
    bash
    npm install
    # or
    yarn install
    # or
    pnpm install
    
5.  **Set Up Pre-commit Hooks:**
    bash
    npm run prepare
    # or
    yarn prepare
    # or
    pnpm prepare
    
    This installs linters and formatters (Biome) to ensure code quality before commits.

## 4. Development Workflow

We follow a strict development loop to ensure code quality and velocity:

1.  **Create a Branch:** Always create a new branch for your feature or fix.
    bash
    git checkout -b feat/your-feature-name
    # or
    git checkout -b fix/your-bug-fix
    
2.  **Code:** Implement your changes. Follow the project's coding standards (see Section 5).
3.  **Test:** Write comprehensive unit and integration tests for your changes. Ensure 100% branch coverage.
    *   **Extension Tests:** `npm run test:extension` (using Vitest)
    *   **API Tests:** `npm run test:api` (using Vitest)
    *   **E2E Tests:** `npx playwright test`
4.  **Lint & Format:** Run the linter and formatter.
    bash
    npm run lint
    npm run format
    
    The pre-commit hooks will automatically run these on `git commit`.
5.  **Build:** Ensure the project builds successfully.
    *   **Extension Build:** `npm run build:extension`
    *   **API Build:** `npm run build:api`
6.  **Commit:** Commit your changes using **Conventional Commits**.
    bash
    git commit -m "feat: Implement user profile page"
    # or
    git commit -m "fix: Resolve null pointer in sentiment analysis"
    
7.  **Push:** Push your branch to your fork.
    bash
    git push origin feat/your-feature-name
    
8.  **Open a Pull Request:** Create a Pull Request against the `main` branch of the `chirag127/AuraMind-AI-Emotional-Telemetry-Platform` repository.

## 5. Coding Standards & Principles

*   **Language:** TypeScript (Strict Mode). Use the latest stable ECMAScript features.
*   **Architecture:** Follow the FSD (Feature-Sliced Design) pattern for the extension and a Modular Monolith/Microservices approach for the API. Adhere to SOLID principles.
*   **Tooling:** Use Vite for building, Biome for linting/formatting, Vitest for unit tests, and Playwright for E2E tests.
*   **AI Integration:** If developing AI features, adhere to the [AGENTS.md](https://github.com/chirag127/AuraMind-AI-Emotional-Telemetry-Platform/blob/main/AGENTS.md) directives, prioritizing privacy and responsible AI practices.
*   **Code Style:** Self-documenting code is paramount. Avoid unnecessary comments. Use clear, descriptive names (camelCase for JS/TS).
*   **Error Handling:** Implement robust error handling. Use `try-catch-finally` blocks and fail fast.
*   **Security:** Adhere to DevSecOps principles (OWASP Top 10 2025). Sanitize all inputs.

## 6. Pull Request Process

*   **Target Branch:** All PRs should target the `main` branch.
*   **Description:** Provide a clear and concise description of your changes, including the problem solved and the solution implemented.
*   **Tests:** Ensure all tests are passing and new tests cover your changes.
*   **CI/CD:** All PRs will be checked by automated CI/CD pipelines. Do not merge until all checks pass.
*   **Reviews:** Expect at least one reviewer to approve your PR. Be receptive to feedback.

## 7. Reporting Issues

*   **Bug Reports:** Please use the provided [Bug Report Template](https://github.com/chirag127/AuraMind-AI-Emotional-Telemetry-Platform/issues/new?template=bug_report.md).
    *   Include a clear title.
    *   Provide steps to reproduce the bug.
    *   Describe the expected and actual behavior.
    *   Include relevant logs, screenshots, or error messages.
*   **Feature Requests:** Feel free to open an issue detailing your proposed feature.

## 8. Community

Join our community discussions on GitHub Discussions or other platforms (TBD). Let's build a privacy-first AI emotional telemetry platform together!

By contributing, you agree that your contributions will be licensed under the terms of the [LICENSE](https://github.com/chirag127/AuraMind-AI-Emotional-Telemetry-Platform/blob/main/LICENSE) file (CC BY-NC).
