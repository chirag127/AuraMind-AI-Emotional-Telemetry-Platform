# AuraMind: AI-Powered Emotional Telemetry Platform

<p align="center">
  <img src="https://img.shields.io/badge/User-%40chirag127-blue?style=flat-square" alt="User">
  <a href="https://github.com/chirag127/AuraMind-AI-Emotional-Telemetry-Platform/actions/workflows/ci.yml">
    <img src="https://img.shields.io/github/actions/workflow/status/chirag127/AuraMind-AI-Emotional-Telemetry-Platform/ci.yml?style=flat-square&label=Build">
  </a>
  <a href="https://codecov.io/gh/chirag127/AuraMind-AI-Emotional-Telemetry-Platform">
    <img src="https://img.shields.io/codecov/c/github/chirag127/AuraMind-AI-Emotional-Telemetry-Platform?style=flat-square&token=XYZ123">
  </a>
  <img src="https://img.shields.io/badge/TechStack-JS%7CRust%7CTailwind-brightgreen?style=flat-square" alt="Tech Stack">
  <img src="https://img.shields.io/badge/Lint%2FFormat-Biome-yellow?style=flat-square" alt="Lint/Format">
  <img src="https://img.shields.io/badge/License-CC%20BY--NC%204.0-orange?style=flat-square" alt="License">
  <a href="https://github.com/chirag127/AuraMind-AI-Emotional-Telemetry-Platform/stargazers">
    <img src="https://img.shields.io/github/stars/chirag127/AuraMind-AI-Emotional-Telemetry-Platform?style=flat-square" alt="GitHub Stars">
  </a>
</p>

<p align="center">
  <a href="https://github.com/chirag127/AuraMind-AI-Emotional-Telemetry-Platform/issues">
    <img src="https://img.shields.io/github/issues/chirag127/AuraMind-AI-Emotional-Telemetry-Platform?style=flat-square&label=Issues" alt="GitHub Issues">
  </a>
  <a href="https://github.com/chirag127/AuraMind-AI-Emotional-Telemetry-Platform/pulls">
    <img src="https://img.shields.io/github/issues-pr/chirag127/AuraMind-AI-Emotional-Telemetry-Platform?style=flat-square&label=Pull%20Requests" alt="GitHub Pull Requests">
  </a>
</p>

<p align="center">
  Star ⭐ this Repo!
</p>

---

## 🧠 AuraMind: Privacy-First AI Emotional Telemetry

AuraMind is a revolutionary, privacy-first platform designed for capturing and analyzing emotional telemetry. It operates using a Manifest V3 browser extension that processes data locally, ensuring user privacy. An optional, self-hostable Node.js API enhances this by providing advanced sentiment analysis and visualization capabilities, tracking emotional states across web sessions without compromising data confidentiality.

---

## 🌳 Architecture

AuraMind employs a modular architecture combining a core browser extension (WXT Framework, TypeScript) with an optional Node.js API backend.

mermaid
graph TD
    A[User Browser]
    B(Manifest V3 Extension)
    C{Local Data Processing}
    D[Optional API Server]
    E(Node.js / Rust)
    F[Advanced Sentiment Analysis]
    G[Visualization Service]
    H[Database Storage]

    A --> B
    B --> C
    C -- Encrypted/Anonymized Data --> D
    D -- API Endpoint --> F
    D -- API Endpoint --> G
    F --> H
    G --> H
    D -- User Interface --> I[Client Application]

    subgraph Extension
        B
        C
    end

    subgraph API Server
        D
        E
        F
        G
        H
    end

    style Extension fill:#cce5ff,stroke:#007bff,stroke-width:2px
    style API Server fill:#e2ffe5,stroke:#28a745,stroke-width:2px


---

## 📜 Table of Contents

*   [Features](#features)
*   [Tech Stack](#tech-stack)
*   [Getting Started](#getting-started)
*   [Development](#development)
*   [Testing](#testing)
*   [Contribution](#contribution)
*   [License](#license)
*   [Security](#security)
*   *   [AI Agent Directives](#ai-agent-directives)

---

## ✨ Features

*   **Privacy-First Design:** All core telemetry processing occurs locally within the browser extension.
*   **Manifest V3 Compatible:** Built to adhere to the latest Chrome Extension standards.
*   **Local Data Handling:** Captures and analyzes emotional states without sending raw user data externally.
*   **Optional API:** Provides enhanced sentiment analysis, visualization, and historical tracking via a secure, self-hostable Node.js API.
*   **Cross-Platform Extension:** Utilizes the WXT Framework for seamless development across multiple browsers.
*   **Modular Development:** Clear separation between extension and API concerns.

---

## 🛠️ Tech Stack

*   **Browser Extension:**
    *   **Framework:** WXT (Web Extension Toolkit)
    *   **Language:** TypeScript (Strict Mode)
    *   **Build Tool:** Vite (Rolldown)
    *   **Styling:** Tailwind CSS v4
    *   **Runtime:** Browser Native (Manifest V3)
*   **Optional API Server:**
    *   **Language:** Node.js (v20+)
    *   **Framework:** Express.js (or similar lightweight framework)
    *   **AI Integration:** Libraries for sentiment analysis (e.g., `compromise`, `natural`, or direct API calls).
    *   **Data Storage:** PostgreSQL / MongoDB (configurable)
*   **Development & CI/CD:**
    *   **Package Manager:** npm / yarn / pnpm
    *   **Linter/Formatter:** Biome
    *   **Testing:** Vitest (Unit/Integration), Playwright (E2E)
    *   **CI/CD:** GitHub Actions

---

## 🚀 Getting Started

### Prerequisites

*   Node.js (v20+)
*   npm / yarn / pnpm
*   Rust (for WXT native tooling, if applicable)

### Installation

1.  **Clone the repository:**
    bash
    git clone https://github.com/chirag127/AuraMind-AI-Emotional-Telemetry-Platform.git
    cd AuraMind-AI-Emotional-Telemetry-Platform
    

2.  **Install Extension Dependencies:**
    bash
    npm install --filter=@auramind/extension
    # or yarn install --filter=@auramind/extension
    

3.  **Install API Dependencies (Optional):**
    bash
    npm install --filter=@auramind/api
    # or yarn install --filter=@auramind/api
    

---

## 💻 Development

### Running the Extension

*   **Development Server:**
    bash
    npm run dev --filter=@auramind/extension
    
    Follow WXT instructions to load the unpacked extension in your browser.

*   **Building for Production:**
    bash
    npm run build --filter=@auramind/extension
    

### Running the API Server (Optional)

*   **Development Server:**
    bash
    npm run dev --filter=@auramind/api
    

*   **Building for Production:**
    bash
    npm run build --filter=@auramind/api
    

---

## 🧪 Testing

### Running Tests

*   **Extension Tests:**
    bash
    npm run test --filter=@auramind/extension
    

*   **API Tests:**
    bash
    npm run test --filter=@auramind/api
    

*   **End-to-End Tests (Playwright):**
    bash
    npm run test:e2e --filter=@auramind/extension
    # or similar for API if applicable
    

---

## 🤝 Contribution

Contributions are welcome! Please follow the guidelines outlined in [CONTRIBUTING.md](/.github/CONTRIBUTING.md).

---

## ⚖️ License

This project is licensed under the **Creative Commons Attribution-NonCommercial 4.0 International License (CC BY-NC 4.0)**. See the [LICENSE](LICENSE) file for more details.

---

## 🛡️ Security

Security is paramount. Please refer to our [SECURITY.md](/.github/SECURITY.md) guidelines for reporting vulnerabilities.

---

## 🤖 AI Agent Directives

<details>
<summary>Click to expand AI Agent Directives</summary>

This section outlines the core directives for AI agents interacting with the **AuraMind** repository, ensuring alignment with its architectural principles and operational standards.

### 1. Identity & Prime Directive

*   **Role:** You are a Senior Principal Software Architect and Master Technical Copywriter with **40+ years of elite industry experience**. You operate with absolute precision, enforcing FAANG-level standards and the wisdom of "Managing the Unmanageable."
*   **Context:** Current Date is **December 2025**. You are building for the 2026 standard.
*   **Output Standard:** Deliver **EXECUTION-ONLY** results. No plans, no "reporting"—only executed code, updated docs, and applied fixes.
*   **Philosophy:** "Zero-Defect, High-Velocity, Future-Proof."

### 2. Input Processing & Cognition

*   **Speech-to-Text Interpretation Protocol:**
    *   **Context:** User inputs may contain phonetic errors (homophones, typos).
    *   **Semantic Correction:** **STRICTLY FORBIDDEN** from executing literal typos. You must **INFER** technical intent based on the project context.
    *   **Logic Anchor:** Treat the `README.md` as the **Single Source of Truth (SSOT)**.
*   **Mandatory MCP Instrumentation:**
    *   **No Guessing:** Do not hallucinate APIs.
    *   **Research First:** Use `linkup`/`brave` to search for **December 2025 Industry Standards**, **Security Threats**, and **2026 UI Trends**.
    *   **Validation:** Use `docfork` to verify *every* external API signature.
    *   **Reasoning:** Engage `clear-thought-two` to architect complex flows *before* writing code.

### 3. Context-Aware Apex Tech Stacks (Late 2025 Standards)

*   **Project Type:** **Browser Extension & Optional API Server**
*   **Primary Stack (Extension):**
    *   **Framework:** WXT (Web Extension Toolkit)
    *   **Language:** TypeScript (Strict Mode)
    *   **Build Tool:** Vite (Rolldown)
    *   **Styling:** Tailwind CSS v4
    *   **Runtime:** Browser Native (Manifest V3)
*   **Secondary Stack (API):**
    *   **Language:** Node.js (v20+)
    *   **Framework:** Express.js (or similar)
    *   **AI Integration:** Sentiment analysis libraries or cloud APIs.
*   **Architecture:** Modular design with clear separation between extension and API concerns. Adheres to **Feature-Sliced Design (FSD)** principles for the extension.

### 4. Development & Workflow Standards

*   **Package Management:** npm / yarn / pnpm.
*   **Linting & Formatting:** **Biome** is the mandatory tool for code quality enforcement across all JavaScript/TypeScript/JSON/YAML files.
*   **Version Control:** Git.
*   **CI/CD:** GitHub Actions. Ensure `ci.yml` is robust and covers build, lint, test, and deployment stages.

### 5. Testing Strategy

*   **Unit & Integration Testing:** **Vitest** is the primary framework.
*   **End-to-End (E2E) Testing:** **Playwright** for comprehensive browser automation testing.
*   **Coverage:** Aim for >80% code coverage. Integrate with Codecov.

### 6. Data Handling & Privacy

*   **Core Principle:** **Privacy by Design**. All sensitive user data must be processed locally within the extension whenever possible.
*   **API Data:** Any data transmitted to or processed by the optional API must be anonymized or pseudonymized, respecting user consent and privacy regulations.
*   **Encryption:** Use industry-standard encryption for data at rest and in transit.

### 7. AI Integration Protocols

*   **Sentiment Analysis:** Utilize optimized libraries or cloud APIs for accurate sentiment detection.
*   **Modularity:** AI components must be isolated and adhere to clean API contracts.
*   **Performance:** Ensure AI processing is efficient, especially within the extension's local environment.

### 8. Output Formatting

*   **Code:** Adhere to Biome's formatting standards.
*   **Documentation:** Maintain clear, concise, and up-to-date documentation.
*   **Commits:** Follow Conventional Commits specification.

</details>
