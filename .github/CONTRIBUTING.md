# 🤝 Contributing to AuraMind-AI-Emotional-Telemetry-Platform

Thank you for considering contributing to AuraMind! We welcome contributions from everyone, whether it's bug reports, feature requests, documentation improvements, or code. To ensure a smooth and productive experience for all, please follow these guidelines.

## 1. Our Philosophy & Standards

This project adheres to the **Apex Technical Authority** standards, emphasizing **Zero-Defect, High-Velocity, Future-Proof** development. This means we value:

*   **Clarity:** Well-documented code and clear communication.
*   **Quality:** Robust testing, strict linting, and adherence to architectural principles (SOLID, DRY, YAGNI).
*   **Security:** Privacy-by-design is paramount, especially given the sensitive nature of emotional telemetry.
*   **Efficiency:** Leveraging modern tooling for rapid development and stable builds.

For detailed technical directives, please refer to our `AGENTS.md`.

## 2. Getting Started

### 2.1. Prerequisites

Before you can contribute, ensure you have the following installed:

*   **Git:** For version control.
*   **Node.js & npm/yarn/pnpm:** For the browser extension development (`wxt` framework).
*   **Node.js (LTS version):** For the optional API backend.

Refer to `README.md` for specific version requirements.

### 2.2. Cloning the Repository

Clone the repository locally using your preferred Git client:

bash
git clone https://github.com/chirag127/AuraMind-AI-Emotional-Telemetry-Platform.git
cd AuraMind-AI-Emotional-Telemetry-Platform


### 2.3. Setting Up the Development Environment

Follow the setup instructions in the `README.md` to install dependencies and configure the development environment for both the browser extension and the Node.js API.

## 3. How to Contribute

### 3.1. Reporting Bugs

If you find a bug, please submit an issue using the `Bug Report` template. Provide as much detail as possible:

*   **Clear Title:** Briefly describe the bug.
*   **Steps to Reproduce:** Detailed, step-by-step instructions.
*   **Expected Behavior:** What should have happened?
*   **Actual Behavior:** What actually happened?
*   **Environment:** Browser/OS, Node.js version, relevant configuration.
*   **Screenshots/Logs:** If applicable.

### 3.2. Suggesting Enhancements or Features

Use the `Feature Request` issue template. Explain the proposed feature and its benefits. If you're willing to implement it, please mention that in your request!

### 3.3. Contributing Code

1.  **Fork the Repository:** Create a personal fork of the `chirag127/AuraMind-AI-Emotional-Telemetry-Platform` repository.
2.  **Create a Feature Branch:** Branch off the `main` branch for your new feature or bug fix (e.g., `git checkout -b feature/my-new-feature` or `git checkout -b fix/bug-description`).
3.  **Make Your Changes:** Implement your code, ensuring it adheres to project standards.
4.  **Test Your Changes:** Write and run tests to verify your code. Ensure all existing tests pass.
5.  **Lint and Format:** Run the linter and formatter (`npx @biomejs/biome format --write .` and `npx @biomejs/biome lint --apply .`) to ensure code style consistency.
6.  **Commit Your Changes:** Write clear, concise commit messages. Follow conventional commits if possible.
7.  **Push to Your Fork:** Push your branch to your fork (e.g., `git push origin feature/my-new-feature`).
8.  **Open a Pull Request:** Submit a pull request against the `main` branch of the `chirag127/AuraMind-AI-Emotional-Telemetry-Platform` repository. Provide a clear description of your changes.

#### 3.3.1. Code Style & Quality

*   **Language:** JavaScript/TypeScript
*   **Linter/Formatter:** Biome (`@biomejs/biome`)
*   **Testing:** Vitest (Unit/Integration), Playwright (E2E)
*   **Architecture:** Follows principles outlined in `AGENTS.md` (e.g., modularity, privacy-first).

### 3.4. Documentation

Well-documented code is crucial. Please update or add documentation for any new features or significant changes. This includes:

*   Code comments for complex logic.
*   Updates to the `README.md` if the user experience changes.
*   Updates to `AGENTS.md` if new technical directives are introduced.

## 4. Pull Request Process

*   **One Request, One Goal:** Each pull request should address a single concern (bug fix, feature).
*   **Clear Descriptions:** Explain *what* the change is and *why* it's needed.
*   **Link to Issues:** Reference any related issues using keywords like `Fixes #123` or `Closes #456`.
*   **Code Reviews:** Expect constructive feedback during code review. Be open to suggestions and willing to make necessary changes.
*   **CI/CD:** Automated checks will run on your PR. Ensure all checks pass before merging.

## 5. Communication

*   **Issues:** Use GitHub Issues for bug reports, feature requests, and discussions.
*   **Pull Requests:** Use PRs for code contributions.
*   **Discussions:** For broader topics or questions not suitable for issues, consider using GitHub Discussions if enabled.

## 6. Code of Conduct

This project is governed by a Code of Conduct (if applicable, otherwise state that we adhere to general respectful communication). We expect all contributors to uphold these standards. Please treat everyone with respect and professionalism.

## 7. Maintainers

*   **chirag127**

Thank you again for contributing!
