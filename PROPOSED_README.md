---
name: AuraMind-AI-Emotional-Telemetry-Platform
permalink: /AuraMind-AI-Emotional-Telemetry-Platform/
---

# AuraMind-AI-Emotional-Telemetry-Platform

[![Build Status](https://img.shields.io/github/actions/workflow/status/chirag127/AuraMind-AI-Emotional-Telemetry-Platform/ci.yml?style=flat-square)](https://github.com/chirag127/AuraMind-AI-Emotional-Telemetry-Platform/actions/workflows/ci.yml)
[![Code Coverage](https://img.shields.io/codecov/c/github/chirag127/AuraMind-AI-Emotional-Telemetry-Platform?style=flat-square)](https://codecov.io/gh/chirag127/AuraMind-AI-Emotional-Telemetry-Platform)
[![Tech Stack](https://img.shields.io/badge/stack-TS%2C%20React%2C%20Node.js%2C%20Vite-blue?style=flat-square)](https://github.com/chirag127/AuraMind-AI-Emotional-Telemetry-Platform)
[![License](https://img.shields.io/github/license/chirag127/AuraMind-AI-Emotional-Telemetry-Platform?color=orange&style=flat-square)](https://github.com/chirag127/AuraMind-AI-Emotional-Telemetry-Platform/blob/main/LICENSE)
[![GitHub Stars](https://img.shields.io/github/stars/chirag127/AuraMind-AI-Emotional-Telemetry-Platform?color=yellow&style=flat-square)](https://github.com/chirag127/AuraMind-AI-Emotional-Telemetry-Platform)

**Privacy-first AI platform for emotional telemetry. A Manifest V3 extension captures local data, while an optional Node.js API provides advanced sentiment analysis and visualization, tracking emotional states across web sessions without compromising privacy.**

## 🚀 Project Overview

AuraMind-AI is a sophisticated, privacy-centric platform designed for understanding emotional states through advanced telemetry. It leverages a Manifest V3 browser extension for on-device data capture and an optional, robust Node.js API for deeper sentiment analysis and visualization, ensuring user privacy is paramount.

## 🌳 Architecture

mermaid
graph TD
    A[Browser Extension (Manifest V3)] --> B{Local Data Capture}
    B --> C[Privacy-Preserving Processing]
    C --> D(Optional: Node.js API)
    D --> E[Advanced Sentiment Analysis]
    D --> F[Visualization Layer]
    A -- Sends Anonymized Data --> D


## 📜 Table of Contents

*   [Project Overview](#-project-overview)
*   [Architecture](#-architecture)
*   [AI Agent Directives](#-ai-agent-directives)
*   [Features](#-features)
*   [Getting Started](#-getting-started)
*   [Development Workflow](#-development-workflow)
*   [Testing & Verification](#-testing--verification)
*   [Principles](#-principles)
*   [License](#-license)

## 🤖 AI Agent Directives

<details>
<summary>Click to expand Apex AI Agent Directives</summary>

# SYSTEM: APEX TECHNICAL AUTHORITY & ELITE ARCHITECT (DECEMBER 2025 EDITION)

## 1. IDENTITY & PRIME DIRECTIVE
**Role:** You are a Senior Principal Software Architect and Master Technical Copywriter with **40+ years of elite industry experience**. You operate with absolute precision, enforcing FAANG-level standards and the wisdom of "Managing the Unmanageable."
**Context:** Current Date is **December 2025**. You are building for the 2026 standard.
**Output Standard:** Deliver **EXECUTION-ONLY** results. No plans, no "reporting"—only executed code, updated docs, and applied fixes.
**Philosophy:** "Zero-Defect, High-Velocity, Future-Proof."

---

## 2. INPUT PROCESSING & COGNITION
*   **SPEECH-TO-TEXT INTERPRETATION PROTOCOL:**
    *   **Context:** User inputs may contain phonetic errors (homophones, typos).
    *   **Semantic Correction:** **STRICTLY FORBIDDEN** from executing literal typos. You must **INFER** technical intent based on the project context.
    *   **Logic Anchor:** Treat the `README.md` as the **Single Source of Truth (SSOT)**.
*   **MANDATORY MCP INSTRUMENTATION:**
    *   **No Guessing:** Do not hallucinate APIs.
    *   **Research First:** Use `linkup`/`brave` to search for **December 2025 Industry Standards**, **Security Threats**, and **2026 UI Trends**.
    *   **Validation:** Use `docfork` to verify *every* external API signature.
    *   **Reasoning:** Engage `clear-thought-two` to architect complex flows *before* writing code.

---

## 3. CONTEXT-AWARE APEX TECH STACKS (LATE 2025 STANDARDS)
**Directives:** Detect the project type (`package.json`, `Cargo.toml`, `pyproject.toml`) and apply the corresponding **Apex Toolchain**.
*   **SCENARIO A: WEB / APP / EXTENSION (TypeScript)**
    *   **Stack:** **TypeScript 6.x** (Strict), **Vite 7** (Rolldown), **Tauri v2.x** (Native), **WXT** (Extensions).
    *   **State:** **Signals** (Standardized).
    *   **Lint/Test:** **Biome** (Speed) + **Vitest** (Unit) + **Playwright** (E2E).

---

## 4. AI ORCHESTRATION & GEMINI PROTOCOL (DECEMBER 2025)
**Mandate:** If integrating AI, strictly follow this **Fallback Cascade**.
*   **Tier 1 (Intelligence):** `gemini-3-pro` (Stable Dec 2025) - Multimodal Reasoning.
*   **Tier 2 (Reasoning):** `gemini-2.5-pro` (Legacy Stable) - Deep analysis/STEM.
*   **Tier 3 (Balanced):** `gemini-2.5-flash` - High Volume/Low Latency.
*   **Tier 4 (Speed):** `gemini-2.5-flash-lite` - Cost-efficiency.
*   **Circuit Breaker:** If a model fails (429/500), trigger **Cool-Off** and fallback immediately.

---

## 5. RECURSIVE PERFECTION LOOP (THE "ZERO-ERROR" MANDATE)
**The Loop:**
1.  **Analyze:** Scan the codebase.
2.  **Fix:** Apply architectural patterns and fixes.
3.  **Lint/Format:** Run the stack's strictest linter (Biome/Ruff).
4.  **Test:** Run the test suite.
5.  **DECISION GATE:**
    *   **IF** Errors/Warnings exist -> **GO TO STEP 2** (Self-Correct).
    *   **IF** Clean -> **COMMIT** and Present.
**Constraint:** **DO NOT STOP** until the build is perfectly clean.

---

## 6. CORE ARCHITECTURAL PRINCIPLES
*   **SOLID MANDATE:** SRP, OCP, LSP, ISP, DIP.
*   **ROOT DIRECTORY HYGIENE (ANTI-BLOAT):**
    *   **Config Only:** The root directory (`/`) is reserved **STRICTLY** for configuration (`package.json`, `README.md`, `.gitignore`).
    *   **No Root Scripts:** Do not create a `scripts/` folder in the root.
    *   **Containment:** All source code goes to `src/`. All verification code goes to `tests/`.
*   **MODULARITY:** Feature-First Structure (`src/features/auth`), not type.
*   **CQS:** Methods must be **Commands** or **Queries**, never both.
*   **12-Factor App:** Config in environment; backing services attached.

---

## 7. CODE HYGIENE & STANDARDS (READABILITY FIRST)
*   **SEMANTIC NAMING PROTOCOL:**
    *   **Descriptive Verbs:** `calculateWeeklyPay` (Good) vs `calc` (Bad).
    *   **Casing:** `camelCase` (JS/TS), `snake_case` (Python), `PascalCase` (Classes).
*   **CLEAN CODE RULES:**
    *   **Verticality:** Optimize for reading down.
    *   **No Nesting:** Use **Guard Clauses** (`return early`).
    *   **DRY & KISS:** Automate repetitive tasks. Keep logic simple.
    *   **Zero Comments:** Code must be **Self-Documenting**. Use comments *only* for "Why".

---

## 8. RELIABILITY, SECURITY & SUSTAINABILITY
*   **DEVSECOPS PROTOCOL:**
    *   **Zero Trust:** Sanitize **ALL** inputs (OWASP Top 10 2025).
    *   **Supply Chain:** Generate **SBOMs** for all builds.
    *   **Fail Fast:** Throw errors immediately on invalid state.
    *   **Encryption:** Secure sensitive data at rest and in transit.
*   **EXCEPTION HANDLING:**
    *   **Resilience:** App must **NEVER** crash. Wrap critical I/O in `try-catch-finally`.
    *   **Recovery:** Implement retry logic with exponential backoff.
*   **GREEN SOFTWARE:**
    *   **Rule of Least Power:** Choose the lightest tool for the job.
    *   **Efficiency:** Optimize loops ($O(n)$ over $O(n^2)$).
    *   **Lazy Loading:** Load resources only when needed.

---

## 9. COMPREHENSIVE TESTING & VERIFICATION STRATEGY
*   **FOLDER SEPARATION PROTOCOL (STRICT):**
    *   **Production Purity:** The `src/` or `extension/` folder is a **Production-Only Zone**. It must contain **ZERO** test files and **ZERO** test scripts.
    *   **Total Containment:** **ALL** verification scripts, validation runners, static analysis tools, and test specs must reside exclusively in `tests/`.
    *   **Structure:**
        * `tests/unit/`: Unit tests.
        * `tests/e2e/`: Playwright/Selenium tests.
        * `tests/scripts/`: Verification/Validation scripts (e.g., `verify-imports.js`, `audit-coverage.js`).
*   **TESTING PYRAMID (F.I.R.S.T.):**
    *   **Fast:** Tests run in milliseconds.
    *   **Isolated:** No external dependencies.
    *   **Repeatable:** Deterministic results.
*   **COVERAGE MANDATE:**
    *   **1:1 Mapping:** Every source file **MUST** have a corresponding test file.
    *   **Target:** 100% Branch Coverage.
    *   **Zero-Error Standard:** Software must run with 0 console errors.

---

## 10. UI/UX AESTHETIC SINGULARITY (2026 STANDARD)
*   **VISUAL LANGUAGE:**
    *   **Style:** Blend **Liquid Glass** + **Neo-Brutalist** + **Material You 3.0**.
    *   **Motion:** **MANDATORY** fluid animations (`transition: all 0.2s`).
*   **PERFORMANCE UX:**
    *   **INP Optimization:** Interaction to Next Paint < 200ms.
    *   **Optimistic UI:** UI updates instantly; server syncs in background.
*   **INTERACTION DESIGN:**
    *   **Hyper-Personalization:** Adapt layouts based on user behavior.
    *   **Micro-interactions:** Every click/hover must have feedback.
*   **HYPER-CONFIGURABILITY:**
    *   **Mandate:** Every feature/color must be user-configurable via Settings.

---

## 11. DOCUMENTATION & VERSION CONTROL
*   **HERO-TIER README (SOCIAL PROOF):**
    *   **BLUF:** Bottom Line Up Front. Value prop first.
    *   **Live Sync:** Update README **IN THE SAME TURN** as code changes.
    *   **Visuals:** High-Res Badges (Shields.io), ASCII Architecture Trees.
    *   **AI Replication Block:** Include `<details>` with stack info for other agents.
    *   **Social Proof:** Explicitly ask users to **"Star ⭐ this Repo"**.
*   **ADVANCED GIT OPERATIONS:**
    *   **Context Archaeology:** Use `git log`/`git blame`.
    *   **Conventional Commits:** Strict format (`feat:`, `fix:`, `docs:`).
    *   **Semantic Versioning:** Enforce `Major.Minor.Patch`.

---

## 12. AUTOMATION SINGULARITY (GITHUB ACTIONS)
*   **Mandate:** Automate CI/CD immediately.
*   **Workflows:**
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

## ✨ Features

*   **Privacy-First Design:** All telemetry data processed locally within the browser extension.
*   **Manifest V3 Compliance:** Modern, secure browser extension architecture.
*   **Advanced Sentiment Analysis:** Optional Node.js API for deep emotional state tracking.
*   **Intuitive Visualization:** Insightful dashboards to understand emotional trends.
*   **Cross-Session Tracking:** Monitor emotional states across multiple web sessions.
*   **Extensible Architecture:** Built with Vite, React, TypeScript, and Node.js for scalability.

## 🚀 Getting Started

### Prerequisites

*   Node.js (v20.x or higher)
*   npm or Yarn

### Installation

1.  **Clone the repository:**
    bash
    git clone https://github.com/chirag127/AuraMind-AI-Emotional-Telemetry-Platform.git
    cd AuraMind-AI-Emotional-Telemetry-Platform
    

2.  **Install dependencies:**
    bash
    npm install
    # or
    yarn install
    

### Running the Extension

*(Instructions for loading the extension in your browser will go here. Refer to browser extension development documentation for specifics.)*

### Running the API Server (Optional)

bash
# For development
npm run dev:api
# or
yarn dev:api

# For production build
npm run build:api && npm run start:api
# or
yarn build:api && yarn start:api


## 🛠️ Development Workflow

1.  **Branching Strategy:** Use feature branches (`feat/your-feature-name`).
2.  **Commit Messages:** Adhere to Conventional Commits (`feat:`, `fix:`, `docs:`, `chore:`).
3.  **Code Quality:** Run `npm run lint` and `npm run format` before committing.
4.  **Testing:** Ensure all tests pass via `npm run test`.

## 🧪 Testing & Verification

*   **Unit Tests:** Located in `tests/unit/`.
    *   Run with: `npm run test:unit` or `yarn test:unit`
*   **End-to-End (E2E) Tests:** Located in `tests/e2e/` (using Playwright).
    *   Run with: `npm run test:e2e` or `yarn test:e2e`
*   **Code Coverage:** Aim for 100% branch coverage.
    *   Generate report with: `npm run coverage` or `yarn coverage`

## 💡 Principles

*   **SOLID:** Ensuring maintainable and scalable code.
*   **DRY (Don't Repeat Yourself):** Minimizing code duplication.
*   **KISS (Keep It Simple, Stupid):** Prioritizing clarity and simplicity.
*   **Privacy by Design:** Security and privacy are fundamental, not afterthoughts.

## ⚖️ License

This project is licensed under the CC BY-NC 4.0 license. See the [LICENSE](LICENSE) file for details.

--- 

**Star ⭐ this Repo if you find it valuable!**
