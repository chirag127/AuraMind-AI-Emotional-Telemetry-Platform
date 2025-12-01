<p align="center">
  <a href="https://github.com/chirag127/AuraMind-AI-Emotional-Telemetry-Platform">
    <img src="https://raw.githubusercontent.com/chirag127/.github/main/profile/auramind-banner.png" alt="AuraMind Banner" width="800" height="auto">
  </a>
</p>

<p align="center">
  <em>Privacy-First AI Emotional Telemetry Platform for Web Sessions</em>
</p>

<p align="center">
  <a href="https://github.com/chirag127/AuraMind-AI-Emotional-Telemetry-Platform/actions/workflows/ci.yml">
    <img src="https://img.shields.io/github/actions/workflow/status/chirag127/AuraMind-AI-Emotional-Telemetry-Platform/ci.yml?branch=main&style=flat-square&label=CI%2FCD%20Build" alt="CI/CD Build Status">
  </a>
  <a href="https://codecov.io/gh/chirag127/AuraMind-AI-Emotional-Telemetry-Platform">
    <img src="https://img.shields.io/codecov/c/github/chirag127/AuraMind-AI-Emotional-Telemetry-Platform?style=flat-square&token=YOUR_CODECOV_TOKEN" alt="Code Coverage">
  </a>
  <img src="https://img.shields.io/badge/Tech%20Stack-WXT%20%7C%20React%20%7C%20Node.js%20%7C%20AI-blueviolet?style=flat-square" alt="Tech Stack">
  <img src="https://img.shields.io/badge/Lint%2FFormat-Biome-informational?style=flat-square" alt="Lint/Format: Biome">
  <a href="https://github.com/chirag127/AuraMind-AI-Emotional-Telemetry-Platform/blob/main/LICENSE">
    <img src="https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey?style=flat-square" alt="License: CC BY-NC 4.0">
  </a>
  <a href="https://github.com/chirag127/AuraMind-AI-Emotional-Telemetry-Platform/stargazers">
    <img src="https://img.shields.io/github/stars/chirag127/AuraMind-AI-Emotional-Telemetry-Platform?style=flat-square&cacheSeconds=3600" alt="GitHub Stars">
  </a>
</p>

<p align="center">
  <a href="https://github.com/chirag127/AuraMind-AI-Emotional-Telemetry-Platform/stargazers">
    <img src="https://img.shields.io/badge/Star%20⭐%20this%20Repo-Support%20Our%20Mission-ff69b4?style=for-the-badge&logo=github" alt="Star this repo">
  </a>
</p>

---

## 🚀 AuraMind: Elevating Emotional Telemetry with Privacy-First AI

AuraMind is an advanced, privacy-first AI platform designed for emotional telemetry, offering deep insights into user sentiment across web sessions. It leverages a Manifest V3 browser extension for secure, local data capture and an optional Node.js API for sophisticated AI-driven sentiment analysis and visualization, all while rigorously upholding user privacy.

### 💡 The Vision

In an increasingly digital world, understanding our emotional responses to online interactions can be crucial for mental well-being and improved user experience. AuraMind empowers individuals and researchers to gain insights into emotional states, fostering a more mindful and humane digital environment without compromising personal data.

---

## 🏛️ Architecture Overview

AuraMind operates as a cohesive system, combining a secure, client-side browser extension with an optional powerful backend for advanced analytics. This distributed architecture ensures privacy by design while offering scalable insights.

mermaid
graph TD
    A[User Browser] -->|Captures Interaction Data| B(AuraMind Manifest V3 Extension)
    B -->|Local Storage & Processing| C{Telemetry Data}
    B -->|Optional: Secure API Call| D[AuraMind Node.js Backend API]
    D -->|AI Sentiment Analysis (e.g., Gemini)| E[Processed Emotional Insights]
    E -->|Secure Data Storage| F[Database (e.g., MongoDB, PostgreSQL)]
    D -->|Return Visualizations / Insights| B
    B -->|Display to User| A


-   **Manifest V3 Extension (Frontend):** Built with WXT and React, responsible for secure, local data capture, initial processing, and displaying insights directly in the browser. Emphasizes privacy by performing most operations client-side.
-   **Node.js Backend API (Optional):** A robust Express.js API designed with Hexagonal Architecture for advanced sentiment analysis using AI (e.g., Google Gemini), data aggregation, and secure storage, only when explicit user consent is given.
-   **AI Integration:** Leverages cutting-edge AI models for nuanced emotional analysis, categorizing sentiment and identifying trends.
-   **Privacy-by-Design:** The core principle guiding every architectural decision, ensuring data minimization, user control, and local processing wherever possible.

---

## 📋 Table of Contents

-   [🚀 AuraMind: Elevating Emotional Telemetry with Privacy-First AI](#-auramind-elevating-emotional-telemetry-with-privacy-first-ai)
    -   [💡 The Vision](#-the-vision)
-   [🏛️ Architecture Overview](#️-architecture-overview)
-   [📋 Table of Contents](#-table-of-contents)
-   [🤖 AI AGENT DIRECTIVES: APEX TECHNICAL AUTHORITY PROTOCOL (DECEMBER 2025 EDITION)](#-ai-agent-directives-apex-technical-authority-protocol-december-2025-edition)
-   [🛠️ Getting Started](#️-getting-started)
    -   [Prerequisites](#prerequisites)
    -   [Installation](#installation)
    -   [Development Scripts](#development-scripts)
-   [✅ Testing](#-testing)
-   [🤝 Contributing](#-contributing)
-   [📄 License](#-license)
-   [🛡️ Security](#️-security)
-   [⭐ Star History](#-star-history)

---

<details>
<summary><h2>🤖 AI AGENT DIRECTIVES: APEX TECHNICAL AUTHORITY PROTOCOL (DECEMBER 2025 EDITION)</h2></summary>

# SYSTEM: APEX TECHNICAL AUTHORITY & ELITE ARCHITECT

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
**Directives:** Detect the project type and apply the corresponding **Apex Toolchain**. This repository, `AuraMind-AI-Emotional-Telemetry-Platform`, comprises a Manifest V3 browser extension (frontend) and an optional Node.js backend API.

*   **PRIMARY SCENARIO: WEB / APP / GUI (Modern Frontend & Backend)**
    *   **Frontend Stack (Browser Extension):** Utilizes **WXT** for Manifest V3 extension development, **React 19+** for UI components, and **TypeScript (Strict)** for robust type safety. **Vite 7 (Rolldown)** is the preferred build tool. **TailwindCSS v4** for utility-first styling.
    *   **Backend Stack (Optional Node.js API):** Leverages **Node.js 20+** with **Express.js** (or similar micro-framework) for API development, also using **TypeScript (Strict)** for maintainability.
    *   **Data Layer:** PostgreSQL or MongoDB for data persistence, secured with proper indexing and encryption.
    *   **AI Integration:** Deeply integrated with **Google Gemini API** (`gemini-3-pro` by default) for advanced sentiment analysis and emotional inference. Prioritize modular design, clear API contracts, and robust error handling for all AI model interactions.
    *   **Architecture:**
        *   **Frontend (Extension):** Adheres to **Feature-Sliced Design (FSD)** for a highly modular, scalable, and maintainable frontend architecture within the WXT/React ecosystem.
        *   **Backend (Node.js):** Employs **Hexagonal Architecture (Ports & Adapters)** to ensure domain logic is decoupled from external concerns (database, API, AI services), promoting testability and flexibility.
    *   **Lint/Format:** **Biome** (for both frontend and backend TypeScript/JavaScript code) for ultra-fast and comprehensive linting and formatting.
    *   **Testing:**
        *   **Unit & Integration:** **Vitest** for React components, WXT extension logic, and Node.js backend services.
        *   **End-to-End (E2E):** **Playwright** for robust browser extension E2E testing, simulating user interactions and API calls across different browser environments.
        *   **API Testing:** Supertest with Vitest for Node.js API endpoint validation.

*   **SECONDARY SCENARIO B: SYSTEMS / PERFORMANCE (Not applicable for this project's primary function.)**
    *   **Stack:** Rust (Cargo) or Go (Modules).
    *   **Lint:** Clippy / GolangCI-Lint.
    *   **Architecture:** Hexagonal Architecture (Ports & Adapters).

*   **TERTIARY SCENARIO C: DATA / AI / SCRIPTS (Python) (Only for specific AI model training/data science scripts if separated)**
    *   **Stack:** uv (Manager), Ruff (Linter), Pytest (Test).
    *   **Architecture:** Modular Monolith or Microservices.

---

## 4. APEX NAMING CONVENTION (THE "STAR VELOCITY" ENGINE)
A high-performing name must instantly communicate **Product**, **Function**,  **Platform** and **Type**.

**Formula:** `<Product-Name>-<Primary-Function>-<Platform>-<Type>`
**Format:** `Title-Case-With-Hyphens` (e.g., `ChatFlow-AI-Powered-Real-Time-Chat-Web-App` or `ZenRead-Book-Reader-CLI-Tool`).

**Rules:**
1.  **Length:** 3 to 10 words.
2.  **Keywords:** MUST include high-volume terms.
3.  **Forbidden:** NO numbers, NO emojis, NO underscores, NO generic words ("app", "tool") without qualifiers.

---

## 5. REPOSITORY INTEGRITY & PURPOSE PIVOT PROTOCOL
**Context:** Analyze the fundamental nature of the repository.
**Rules:**
1.  **Identity Preservation:** Respect the existing project type IF it is viable.
2.  **PURPOSE PIVOT:** If the current purpose is weak, vague, or "junk", you are **AUTHORIZED TO PIVOT**. Re-imagine the codebase as a professional tool.
3.  **PROFESSIONAL ARCHIVAL (THE "RETIRED PRODUCT" STANDARD):** If `action` is "ARCHIVE", elevate metadata to highest professional standard.
4.  **Pragmatic Migration:** **OPTIMIZE** the existing stack.

---

## 6. DEVELOPMENT & DEPLOYMENT STANDARDS
*   **Version Control:** GitFlow branching strategy.
*   **CI/CD:** GitHub Actions for automated testing, linting, building, and deployment (e.g., publishing extension to stores, deploying Node.js API to cloud platforms like Vercel, AWS, Google Cloud).
*   **Containerization:** Docker for consistent development and deployment environments for the Node.js backend.
*   **Cloud Agnostic Design:** Backend API should be deployable on various cloud providers.
*   **API Design:** RESTful principles with OpenAPI/Swagger documentation.
*   **Error Handling:** Robust, centralized error handling with detailed logging (e.g., Winston, Pino).
*   **Monitoring & Observability:** Integration with Prometheus/Grafana or cloud-native monitoring tools for both frontend (e.g., Sentry) and backend.

---

## 7. CODE QUALITY & BEST PRACTICES
*   **SOLID Principles:** Strictly adhered to for maintainable and scalable code.
*   **DRY (Don't Repeat Yourself):** Eliminate redundant code.
*   **YAGNI (You Aren't Gonna Need It):** Avoid premature optimization or over-engineering.
*   **Clean Code:** Focus on readability, simplicity, and clear intent.
*   **Type Safety:** Maximize TypeScript's capabilities.
*   **Security:**
    *   **Privacy-by-Design:** All data handling must prioritize user privacy, adhering to principles like data minimization, consent, and secure processing. Manifest V3 compliance is critical.
    *   **Input Validation:** Strict validation on all user and API inputs.
    *   **Authentication/Authorization:** Robust JWT-based or OAuth2 authentication for backend API.
    *   **Dependency Management:** Regularly audit dependencies for vulnerabilities (e.g., `npm audit`, Snyk).
    *   **CORS:** Properly configured for API.
*   **Documentation:** Comprehensive JSDoc for functions/modules, architectural decision records (ADRs), and detailed `README.md`.

---

## 8. VERIFICATION COMMANDS (EXAMPLE - Adapt as needed)
*   **Install Dependencies:** `npm install`
*   **Run Linter:** `npm run lint`
*   **Run Tests (Frontend/Extension):** `npm test` or `npm run test:extension`
*   **Run Tests (Backend):** `npm run test:backend`
*   **Run E2E Tests:** `npm run test:e2e`
*   **Build Project:** `npm run build`
*   **Start Development Server (Extension):** `npm run dev:extension`
*   **Start Development Server (Backend):** `npm run dev:backend`

</details>

---

## 🛠️ Getting Started

Follow these instructions to set up and run AuraMind locally for development and testing.

### Prerequisites

Ensure you have the following installed:

-   [Node.js](https://nodejs.org/en/download/) (v20.x or higher)
-   [npm](https://www.npmjs.com/) (v10.x or higher) or [yarn](https://yarnpkg.com/)
-   [Google Chrome](https://www.google.com/chrome/) (for testing the browser extension)
-   A text editor like [VS Code](https://code.visualstudio.com/)

### Installation

1.  **Clone the repository:**
    bash
    git clone https://github.com/chirag127/AuraMind-AI-Emotional-Telemetry-Platform.git
    cd AuraMind-AI-Emotional-Telemetry-Platform
    

2.  **Install dependencies for the Extension and Backend:**
    This project uses a monorepo-like structure. Navigate into `extension` and `backend` directories to install dependencies.

    bash
    # For the browser extension
    cd extension
    npm install
    cd ..

    # For the Node.js backend API (optional, if you want advanced features)
    cd backend
    npm install
    cd ..
    

3.  **Configure Environment Variables (Backend - if applicable):**
    If you're using the optional backend, create a `.env` file in the `backend/` directory based on `backend/.env.example` and fill in necessary details (e.g., database connection strings, Google Gemini API key).

### Development Scripts

Run these scripts from the respective `extension/` or `backend/` directories:

| Script              | Description                                        | Location   |
| :------------------ | :------------------------------------------------- | :--------- |
| `npm run dev`       | Starts the development server for the extension.   | `extension`|
| `npm run build`     | Builds the production-ready extension.             | `extension`|
| `npm run lint`      | Runs Biome linter and formatter.                   | `extension`, `backend`|
| `npm run test`      | Runs unit and integration tests.                   | `extension`, `backend`|
| `npm run dev:backend`| Starts the backend API in development mode.       | `backend`  |
| `npm run start:prod`| Starts the backend API in production mode.        | `backend`  |

---

## ✅ Testing

AuraMind employs a comprehensive testing strategy to ensure reliability and maintainability.

-   **Unit & Integration Tests:** Utilizes **Vitest** for robust testing of individual components, modules, and service integrations for both the extension and backend.
-   **End-to-End (E2E) Tests:** Leverages **Playwright** for simulating real user interactions with the browser extension across different browsers, verifying full system flows.

To run tests:

bash
# Run all tests for the extension
cd extension
npm test

# Run all tests for the backend
cd backend
npm test


---

## 🤝 Contributing

We welcome contributions to AuraMind! Please see our [CONTRIBUTING.md](https://github.com/chirag127/AuraMind-AI-Emotional-Telemetry-Platform/blob/main/.github/CONTRIBUTING.md) for guidelines on how to get started, report bugs, and propose features.

---

## 📄 License

This project is licensed under the [Creative Commons Attribution-NonCommercial 4.0 International License](https://github.com/chirag127/AuraMind-AI-Emotional-Telemetry-Platform/blob/main/LICENSE) (CC BY-NC 4.0).

---

## 🛡️ Security

AuraMind is built with a strong emphasis on privacy and security. For information on responsible vulnerability disclosure and our security practices, please refer to [SECURITY.md](https://github.com/chirag127/AuraMind-AI-Emotional-Telemetry-Platform/blob/main/.github/SECURITY.md).

---

## ⭐ Star History

[![Star History Chart](https://api.star-history.com/svg?repos=chirag127/AuraMind-AI-Emotional-Telemetry-Platform&type=Date)](https://star-history.com/#chirag127/AuraMind-AI-Emotional-Telemetry-Platform&Date)
