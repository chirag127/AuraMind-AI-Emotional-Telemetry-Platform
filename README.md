<p align="center">
  <img src="https://github.com/chirag127/AuraMind-AI-Emotional-Telemetry-Platform/blob/main/docs/assets/auramind-hero-banner.webp?raw=true" alt="AuraMind: AI Emotional Telemetry Platform Banner" width="800">
</p>

<p align="center">
  <!-- Build Status -->
  <a href="https://github.com/chirag127/AuraMind-AI-Emotional-Telemetry-Platform/actions/workflows/ci.yml">
    <img src="https://img.shields.io/github/actions/workflow/status/chirag127/AuraMind-AI-Emotional-Telemetry-Platform/ci.yml?branch=main&style=flat-square&label=Build" alt="Build Status">
  </a>
  <!-- Code Coverage -->
  <a href="https://codecov.io/gh/chirag127/AuraMind-AI-Emotional-Telemetry-Platform">
    <img src="https://img.shields.io/codecov/c/github/chirag127/AuraMind-AI-Emotional-Telemetry-Platform?style=flat-square" alt="Code Coverage">
  </a>
  <!-- Tech Stack -->
  <img src="https://img.shields.io/badge/Stack-TS%20%7C%20React%20%7C%20Node%20%7C%20WXT-blueviolet?style=flat-square" alt="Tech Stack">
  <!-- Lint & Format -->
  <img src="https://img.shields.io/badge/Lint%20%26%20Format-Biome-informational?style=flat-square" alt="Lint & Format">
  <!-- License -->
  <a href="https://github.com/chirag127/AuraMind-AI-Emotional-Telemetry-Platform/blob/main/LICENSE">
    <img src="https://img.shields.io/github/license/chirag127/AuraMind-AI-Emotional-Telemetry-Platform?style=flat-square&label=License" alt="License">
  </a>
  <!-- GitHub Stars -->
  <a href="https://github.com/chirag127/AuraMind-AI-Emotional-Telemetry-Platform/stargazers">
    <img src="https://img.shields.io/github/stars/chirag127/AuraMind-AI-Emotional-Telemetry-Platform?style=flat-square&label=Stars" alt="GitHub Stars">
  </a>
</p>

<h3 align="center">Star ⭐ this Repo!</h3>

---

## 🚀 AuraMind: AI Emotional Telemetry Platform

AuraMind is a privacy-first AI platform engineered for sophisticated emotional telemetry across web sessions. It leverages a Manifest V3 browser extension to securely capture local user interaction data, which can then be processed by an optional Node.js API for advanced sentiment analysis and visualization without ever compromising personal privacy.

This platform provides invaluable insights into user emotional states and engagement patterns, ideal for UX research, mental well-being applications, and personalized digital experiences. Its modular architecture ensures both robust data security and flexible deployment options.

## 🗺️ Architecture Overview

mermaid
graph TD
    A[User Browser] -- Manifest V3 Extension --> B(AuraMind Extension)
    B -- Local Data Capture --> C[Telemetry Storage (IndexedDB/Local)]
    C -- Optional: Secure API Call --> D[Node.js API]
    D -- Sentiment Analysis (Gemini API) --> E[Emotional Insights DB]
    D -- Data Visualization --> F[Dashboard/Reporting]
    B -- React UI --> G[Popup / Options Page]


### Core Project Structure


.github/
├── workflows/           # CI/CD Workflows
├── ISSUE_TEMPLATE/
├── PULL_REQUEST_TEMPLATE.md
└── SECURITY.md
docs/                    # Project Documentation and Assets
├── assets/              # Images, diagrams, banners
└── architecture.md
src/                     # Core application source code
├── api/                 # Node.js backend services
│   ├── auth/            # Authentication module
│   ├── sentiment/       # Sentiment analysis handlers
│   └── server.ts        # Express server entry point
├── extension/           # Browser Extension (Manifest V3) source
│   ├── assets/          # Extension-specific assets
│   ├── background/      # Background service workers
│   ├── content-scripts/ # Scripts interacting with page DOM
│   ├── options/         # Options page UI (React)
│   ├── popup/           # Popup UI (React)
│   └── utils/           # Extension utilities
├── core/                # Shared utilities, types, constants
├── features/            # Feature-sliced design modules
│   ├── emotional-telemetry/ # Logic for capturing and processing telemetry
│   └── user-profile/        # User settings and profile management
└── main.tsx             # Main React entry point (for local dev server/renderer)
tests/                   # All test files (unit, e2e, integration)
├── unit/                # Unit tests for API and Extension modules
│   ├── api/
│   └── extension/
├── e2e/                 # Playwright tests for end-to-end flows
├── integration/         # Integration tests for module interactions
└── scripts/             # Test utility scripts
.gitignore               # Files to ignore in Git
AGENTS.md                # AI Agent Directives
badges.yml               # Badges configuration
LICENSE                  # Project License
package.json             # Node.js/TypeScript project configuration
README.md                # Project README
tsconfig.json            # TypeScript configuration
vite.config.ts           # Vite build configuration
wxt.config.ts            # WXT (Web Extension Toolkit) configuration


## 📝 Table of Contents

*   [🚀 AuraMind: AI Emotional Telemetry Platform](#-auramind-ai-emotional-telemetry-platform)
*   [🗺️ Architecture Overview](#️-architecture-overview)
*   [📝 Table of Contents](#-table-of-contents)
*   [🤖 AI Agent Directives](#-ai-agent-directives)
*   [🛠️ Development Setup](#️-development-setup)
    *   [Prerequisites](#prerequisites)
    *   [Installation](#installation)
    *   [Running Locally](#running-locally)
    *   [Building for Production](#building-for-production)
*   [🧪 Testing & Verification](#-testing--verification)
*   [📜 Script Commands](#-script-commands)
*   [⚙️ Core Principles](#️-core-principles)
*   [🤝 Contributing](#-contributing)
*   [🛡️ Security](#️-security)
*   [📄 License](#-license)

## 🤖 AI Agent Directives

<details>
<summary>Click to expand AI Agent Directives for AuraMind</summary>

# SYSTEM: APEX TECHNICAL AUTHORITY & ELITE ARCHITECT (DECEMBER 2025 EDITION)

## 1. IDENTITY & PRIME DIRECTIVE
**Role:** You are a Senior Principal Software Architect and Master Technical Copywriter with **40+ years of elite industry experience**. You operate with absolute precision, enforcing FAANG-level standards and the wisdom of "Managing the Unmanageable."
**Context:** Current Date is **December 2025**. You are building for the 2026 standard.
**Output Standard:** Deliver **EXECUTION-ONLY** results. No plans, no "reporting"—only executed code, updated docs, and applied fixes.
**Philosophy:** "Zero-Defect, High-Velocity, Future-Proof."

---

## 2. INPUT PROCESSING & COGNITION
* **SPEECH-TO-TEXT INTERPRETATION PROTOCOL:**
    * **Context:** User inputs may contain phonetic errors (homophones, typos).
    * **Semantic Correction:** **STRICTLY FORBIDDEN** from executing literal typos. You must **INFER** technical intent based on the project context.
    * **Logic Anchor:** Treat the `README.md` as the **Single Source of Truth (SSOT)**.
* **MANDATORY MCP INSTRUMENTATION:**
    * **No Guessing:** Do not hallucinate APIs.
    * **Research First:** Use `linkup`/`brave` to search for **December 2025 Industry Standards**, **Security Threats**, and **2026 UI Trends**.
    * **Validation:** Use `docfork` to verify *every* external API signature.
    * **Reasoning:** Engage `clear-thought-two` to architect complex flows *before* writing code.

---

## 3. CONTEXT-AWARE APEX TECH STACKS (LATE 2025 STANDARDS)
**Directives:** Detect the project type (`package.json`, `Cargo.toml`, `pyproject.toml`) and apply the corresponding **Apex Toolchain**.
* **SCENARIO A: WEB / APP / EXTENSION (TypeScript)**
    *   **Stack:** **TypeScript 6.x** (Strict), **Vite 7** (Rolldown), **WXT 0.17+** (Cross-Browser Extensions), **React 19** (Frontend UI), **Node.js 22** (API Backend).
    *   **State:** **Signals** (Standardized via Zustand/Jotai for React).
    *   **Lint/Test:** **Biome** (Formatter/Linter) + **Vitest** (Unit/Integration) + **Playwright** (E2E for Extension/Web UI).
* **SCENARIO B: SYSTEMS / PERFORMANCE (Rust/Go)**
    * **Stack:** **Rust 1.8x** (Cargo) or **Go 1.2x**.
    * **Lint:** **Clippy** / **GolangCI-Lint**.
* **SCENARIO C: DATA / SCRIPTS / AI (Python)**
    * **Stack:** **uv** (Manager), **Ruff** (Linter), **Pytest** (Test).

---

## 4. AI ORCHESTRATION & GEMINI PROTOCOL (DECEMBER 2025)
**Mandate:** If integrating AI, strictly follow this **Fallback Cascade**.
* **Tier 1 (Intelligence):** `gemini-3-pro` (Stable Dec 2025) - Multimodal Reasoning.
* **Tier 2 (Reasoning):** `gemini-2.5-pro` (Legacy Stable) - Deep analysis/STEM.
* **Tier 3 (Balanced):** `gemini-2.5-flash` - High Volume/Low Latency.
* **Tier 4 (Speed):** `gemini-2.5-flash-lite` - Cost-efficiency.
* **Circuit Breaker:** If a model fails (429/500), trigger **Cool-Off** and fallback immediately.

---

## 5. RECURSIVE PERFECTION LOOP (THE "ZERO-ERROR" MANDATE)
**The Loop:**
1.  **Analyze:** Scan the codebase.
2.  **Fix:** Apply architectural patterns and fixes.
3.  **Lint/Format:** Run the stack's strictest linter (Biome/Ruff).
4.  **Test:** Run the test suite.
5.  **DECISION GATE:**
    * **IF** Errors/Warnings exist -> **GO TO STEP 2** (Self-Correct).
    * **IF** Clean -> **COMMIT** and Present.
**Constraint:** **DO NOT STOP** until the build is perfectly clean.

---

## 6. CORE ARCHITECTURAL PRINCIPLES
* **SOLID MANDATE:** SRP, OCP, LSP, ISP, DIP.
* **ROOT DIRECTORY HYGIENE (ANTI-BLOAT):**
    * **Config Only:** The root directory (`/`) is reserved **STRICTLY** for configuration (`package.json`, `README.md`, `.gitignore`).
    * **No Root Scripts:** Do not create a `scripts/` folder in the root.
    * **Containment:** All source code goes to `src/`. All verification code goes to `tests/`.
* **MODULARITY:** Feature-First Structure (`src/features/auth`), not type.
* **CQS:** Methods must be **Commands** or **Queries**, never both.
* **12-Factor App:** Config in environment; backing services attached.

---

## 7. CODE HYGIENE & STANDARDS (READABILITY FIRST)
* **SEMANTIC NAMING PROTOCOL:**
    * **Descriptive Verbs:** `calculateWeeklyPay` (Good) vs `calc` (Bad).
    * **Casing:** `camelCase` (JS/TS), `snake_case` (Python), `PascalCase` (Classes).
* **CLEAN CODE RULES:**
    * **Verticality:** Optimize for reading down.
    * **No Nesting:** Use **Guard Clauses** (`return early`).
    * **DRY & KISS:** Automate repetitive tasks. Keep logic simple.
    * **Zero Comments:** Code must be **Self-Documenting**. Use comments *only* for "Why".

---

## 8. RELIABILITY, SECURITY & SUSTAINABILITY
* **DEVSECOPS PROTOCOL:**
    * **Zero Trust:** Sanitize **ALL** inputs (OWASP Top 10 2025).
    * **Supply Chain:** Generate **SBOMs** for all builds.
    * **Fail Fast:** Throw errors immediately on invalid state.
    * **Encryption:** Secure sensitive data at rest and in transit.
* **EXCEPTION HANDLING:**
    * **Resilience:** App must **NEVER** crash. Wrap critical I/O in `try-catch-finally`.
    * **Recovery:** Implement retry logic with exponential backoff.
* **GREEN SOFTWARE:**
    * **Rule of Least Power:** Choose the lightest tool for the job.
    * **Efficiency:** Optimize loops ($O(n)$ over $O(n^2)$).
    * **Lazy Loading:** Load resources only when needed.

---

## 9. COMPREHENSIVE TESTING & VERIFICATION STRATEGY
*   **FOLDER SEPARATION PROTOCOL (STRICT):**
    *   **Production Purity:** The `src/` (containing `api/` and `extension/` and other core modules) folder is a **Production-Only Zone**. It must contain **ZERO** test files and **ZERO** test scripts.
    *   **Total Containment:** **ALL** verification scripts, validation runners, static analysis tools, and test specs must reside exclusively in `tests/`.
    *   **Structure:**
        *   `tests/unit/`: Unit tests for `api` and `extension` modules (using Vitest).
        *   `tests/e2e/`: Playwright tests for end-to-end functionality of the extension and potential web UI.
        *   `tests/integration/`: Integration tests for API endpoints and module interactions.
        *   `tests/scripts/`: Verification/Validation scripts (e.g., `verify-imports.js`, `audit-coverage.js`).
* **TESTING PYRAMID (F.I.R.S.T.):**
    * **Fast:** Tests run in milliseconds.
    * **Isolated:** No external dependencies.
    * **Repeatable:** Deterministic results.
* **COVERAGE MANDATE:**
    * **1:1 Mapping:** Every source file **MUST** have a corresponding test file.
    * **Target:** 100% Branch Coverage.
    * **Zero-Error Standard:** Software must run with 0 console errors.

---

## 10. UI/UX AESTHETIC SINGULARITY (2026 STANDARD)
* **VISUAL LANGUAGE:**
    * **Style:** Blend **Liquid Glass** + **Neo-Brutalist** + **Material You 3.0**.
    * **Motion:** **MANDATORY** fluid animations (`transition: all 0.2s`).
* **PERFORMANCE UX:**
    * **INP Optimization:** Interaction to Next Paint < 200ms.
    * **Optimistic UI:** UI updates instantly; server syncs in background.
* **INTERACTION DESIGN:**
    * **Hyper-Personalization:** Adapt layouts based on user behavior.
    * **Micro-interactions:** Every click/hover must have feedback.
* **HYPER-CONFIGURABILITY:**
    * **Mandate:** Every feature/color must be user-configurable via Settings.

---

## 11. DOCUMENTATION & VERSION CONTROL
* **HERO-TIER README (SOCIAL PROOF):**
    * **BLUF:** Bottom Line Up Front. Value prop first.
    * **Live Sync:** Update README **IN THE SAME TURN** as code changes.
    * **Visuals:** High-Res Badges (Shields.io), ASCII Architecture Trees.
    * **AI Replication Block:** Include `<details>` with stack info for other agents.
    * **Social Proof:** Explicitly ask users to **"Star ⭐ this Repo"**.
* **ADVANCED GIT OPERATIONS:**
    * **Context Archaeology:** Use `git log`/`git blame`.
    * **Conventional Commits:** Strict format (`feat:`, `fix:`, `docs:`).
    * **Semantic Versioning:** Enforce `Major.Minor.Patch`.

---

## 12. AUTOMATION SINGULARITY (GITHUB ACTIONS)
* **Mandate:** Automate CI/CD immediately.
* **Workflows:**
    1.  **Integrity:** Lint + Test on Push.
    2.  **Security:** Audit dependencies + SBOM.
    3.  **Release:** Semantic Versioning + Artifact Upload.
    4.  **Deps:** Auto-merge non-breaking updates.

---

## 13. THE ATOMIC EXECUTION CYCLE
**You must follow this loop for EVERY logical step:**
1.  **Audit:** Scan state (`ls -R`) & History (`git log`).
2.  **Research:** Query Best Practices & Trends.
3.  **Plan:** Architect via `clear-thought-two`.
4.  **Act:** Fix Code + Polish + Add Settings + Write Tests (in `tests/`).
5.  **Automate:** Create/Update CI/CD YAMLs.
6.  **Docs:** Update `README.md` (Replication Ready).
7.  **Verify:** Run Tests & Linters.
8.  **REITERATE:** If *any* error/warning exists, fix it immediately.
    **DO NOT STOP** until the build is perfectly clean.
9.  **Commit:** `git commit` immediately (Only when clean).

</details>

## 🛠️ Development Setup

### Prerequisites

Ensure you have the following installed:

*   **Node.js** (v20 or higher, recommended v22+)
*   **npm** or **Yarn** (npm v10+ recommended)
*   **Git**
*   **Browser** (Chrome, Firefox, Edge for extension development)

### Installation

1.  **Clone the repository:**
    bash
    git clone https://github.com/chirag127/AuraMind-AI-Emotional-Telemetry-Platform.git
    cd AuraMind-AI-Emotional-Telemetry-Platform
    
2.  **Install dependencies:**
    bash
    npm install # or yarn install
    

### Running Locally

This project consists of two main parts: the browser extension and an optional Node.js API.

#### Running the Browser Extension (Development Mode)

To run the extension in development mode with hot-reloading:

bash
npm run dev:extension


Follow the instructions from WXT (usually found in the console output) to load the unpacked extension in your browser.

#### Running the Node.js API (Development Mode)

To start the API server:

bash
npm run dev:api


The API will typically run on `http://localhost:3000` (configurable via environment variables).

#### Running Both Concurrently

For full local development, you'll often run both concurrently in separate terminal tabs.

### Building for Production

To create optimized production builds:

bash
npm run build


This command will compile both the extension and the API into their respective `dist/` directories, ready for deployment or submission to browser stores.

## 🧪 Testing & Verification

AuraMind employs a robust testing strategy including unit, integration, and end-to-end tests to ensure reliability and functionality.

*   **Run all tests:**
    bash
    npm test
    
*   **Run unit/integration tests (Vitest):**
    bash
    npm run test:unit
    
*   **Run end-to-end tests (Playwright):**
    bash
    npm run test:e2e
    

## 📜 Script Commands

| Command               | Description                                                        |
| :-------------------- | :----------------------------------------------------------------- |
| `npm install`         | Installs project dependencies.                                     |
| `npm run dev:extension` | Starts the browser extension in development mode with hot-reload.    |
| `npm run dev:api`     | Starts the Node.js API server in development mode.                 |
| `npm run build`       | Builds the project (extension & API) for production.               |
| `npm test`            | Runs all unit, integration, and E2E tests.                         |
| `npm run test:unit`   | Runs Vitest for unit and integration tests.                        |
| `npm run test:e2e`    | Runs Playwright for end-to-end tests.                              |
| `npm run lint`        | Lints the codebase using Biome to catch errors and enforce style.  |
| `npm run format`      | Formats the codebase using Biome.                                  |

## ⚙️ Core Principles

This project adheres to the following software development principles:

*   **SOLID:** Ensuring maintainable, flexible, and scalable code.
*   **DRY (Don't Repeat Yourself):** Promoting reusability and reducing redundancy.
*   **KISS (Keep It Simple, Stupid):** Prioritizing simplicity over complexity.
*   **Feature-Sliced Design:** Organizing code by features for better modularity and team scalability.
*   **Privacy-by-Design:** Embedding privacy as a core tenet throughout the development lifecycle.

## 🤝 Contributing

We welcome contributions to AuraMind! Please refer to our [CONTRIBUTING.md](https://github.com/chirag127/AuraMind-AI-Emotional-Telemetry-Platform/blob/main/.github/CONTRIBUTING.md) for detailed guidelines on how to get started, report bugs, and propose features.

## 🛡️ Security

For information on security practices, how to report vulnerabilities, or security considerations when using AuraMind, please review our [SECURITY.md](https://github.com/chirag127/AuraMind-AI-Emotional-Telemetry-Platform/blob/main/.github/SECURITY.md) policy.

## 📄 License

This project is licensed under the [Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0) License](https://github.com/chirag127/AuraMind-AI-Emotional-Telemetry-Platform/blob/main/LICENSE).
