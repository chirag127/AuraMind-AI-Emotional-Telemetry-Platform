# Security Policy for AuraMind-AI-Emotional-Telemetry-Platform

## 1. Commitment to Security

The **AuraMind-AI-Emotional-Telemetry-Platform** is built on a **Privacy-First** architecture, prioritizing local processing and user data sovereignty. We treat security as a non-negotiable component of our design, adhering to the principle of **Zero Trust** (as defined by the Apex Technical Authority). Security vulnerability reporting follows a rigorous, structured process to ensure rapid mitigation.

--- 

## 2. Supported Versions

| Version | Status | Support Window | Notes |
| :--- | :--- | :--- | :--- |
| `1.x.x` (Current) | Active | Ongoing | Immediate patching for Critical/High severity findings. |
| `0.x.x` (Previous) | Maintenance | 90 Days Post-Release | Only Critical severity vulnerabilities will be backported. |

--- 

## 3. Reporting a Vulnerability

If you discover a security issue, **DO NOT** file a public issue or commit code changes before coordinating with the maintainers. Please follow the structured disclosure process below:

### A. Initial Disclosure (Private Contact)

1.  **Primary Contact:** Please email the Security Team Lead at `security@auramind-platform.dev` (Placeholder).
2.  **Subject Line:** `[SECURITY] Vulnerability Report: [Brief Component Name]`
3.  **Required Information:** Your report must include the following details to facilitate rapid triage (following the **APEX VULNERABILITY SCHEMA**):
    *   **Vulnerability Type:** (e.g., XSS, SSRF, Information Leak, Logic Flaw).
    *   **Affected Component:** (e.g., Browser Extension Manifest V3, Node.js API route `/api/v1/sentiment`).
    *   **Proof of Concept (PoC):** Detailed, non-destructive steps to reproduce the issue.
    *   **Severity Assessment:** Your recommendation based on impact (Critical, High, Medium, Low).
    *   **Data Impact:** Explicitly state if user **PII or emotional telemetry data** is exposed or compromised.

### B. Review and Triage

Upon receipt, the security team will acknowledge your report within **48 hours**. We will assign an internal severity rating and begin immediate remediation efforts under the scope of the **RECURSIVE PERFECTION LOOP**.

### C. Public Disclosure

Public disclosure of the vulnerability and fix will occur **ONLY** after:
1.  A patch has been released to the main branch and deployed to stable channels.
2.  A reasonable grace period (typically 7 days) has passed since the fix deployment, allowing users time to update.

--- 

## 4. Architectural Security Principles (Zero Trust & Privacy)

This project enforces several architectural constraints designed to limit the blast radius of potential vulnerabilities:

*   **Local-First Telemetry:** The primary data processing in the browser extension **MUST** remain client-side (sandboxed) using Manifest V3 service workers. **NO RAW EMOTIONAL DATA** should be sent to the optional API without prior anonymization or user consent flags.
*   **Input Validation:** All data transmitted to the optional Node.js API endpoint **MUST** pass stringent validation checks (e.g., `express-validator` or equivalent) against expected schemas.
*   **Dependency Scanning:** The CI workflow **MUST** execute automated dependency checks (e.g., Snyk or `npm audit`) on every push, blocking merges if High/Critical vulnerabilities are detected.
*   **Secrets Management:** No hardcoded secrets are permitted in the source code. Configuration must rely exclusively on **Environment Variables** (12-Factor App adherence).
*   **API Hardening:** If the optional API is used, it must implement **Rate Limiting** and robust **CORS** policies.

--- 

## 5. Security Tooling in CI/CD

The automated pipeline (`.github/workflows/ci.yml`) is configured to enforce security hygiene at multiple stages:

1.  **Static Analysis (SAST):** Biome (for TS/JS) is run with maximum strictness.
2.  **Dependency Auditing:** Automated checks for known CVEs in dependencies.
3.  **SBOM Generation:** A Software Bill of Materials (SBOM) must be generated for the Node.js backend/API build artifacts.
4.  **CSP Enforcement:** The browser extension manifest must strictly define a Content Security Policy (CSP) that limits external resource loading to an absolute minimum.

*Maintainers: If you introduce a new dependency, ensure its security audit passes before merging.*