# Security Policy for AuraMind-AI-Emotional-Telemetry-Platform

As the Apex Technical Authority, security is treated as a **Tier 0 requirement**, integrated via a strict DevSecOps protocol built on **Zero Trust** principles, adhering to the OWASP Top 10 (2025 standards).

## 1. Supported Versions

This repository actively maintains the latest stable releases for all components:

| Component | Version Status | Notes |
| :--- | :--- | :--- |
| Core Language | TypeScript 6.x | Strict Mode Enabled |
| Frontend Runtime | Vite 7.x | Rollup Backend |
| Browser Extension | Manifest V3 | Strict Content Security Policy enforced. |
| Backend API | Node.js (LTS) | Security auditing via `npm audit` and GitHub Dependabot. |

## 2. Reporting a Vulnerability

We value security researchers and internal developers who report potential vulnerabilities. All reports are treated with the highest level of confidentiality and urgency.

**Reporting Procedure:**

1.  **DO NOT** open a public issue for security concerns.
2.  Immediately send a detailed report via email to: `security@chirag127.dev`.
3.  If reporting externally, please follow our disclosure timeline (Section 3).
4.  Use clear, actionable steps to reproduce the vulnerability (Proof of Concept).

Reports will be acknowledged within **24 hours**.

## 3. Disclosure Policy

We adhere to a responsible disclosure timeline to ensure a fix is available before public knowledge of a vulnerability:

1.  **Triage (0 - 7 days):** Security team analyzes and prioritizes the report.
2.  **Remediation (7 - 45 days):** Development of fix, internal testing, and security hardening.
3.  **Coordinated Public Disclosure (Day 46+):** Once the patch is released (via a new version release), we will coordinate with the reporter, if desired, for joint public acknowledgement.

## 4. Security-Focused Architecture Directives

Security is enforced at multiple layers, especially concerning data telemetry and privacy:

### 4.1. Browser Extension (Manifest V3)
*   **Data Handling:** All emotional telemetry captured is processed **locally** on the client-side whenever possible. No raw, personally identifiable behavioral data leaves the user's machine without explicit, granular consent.
*   **Content Security Policy (CSP):** The extension utilizes the strictest CSP possible, limiting script sources to self-hosted resources and trusted CDNs only. Dynamic code execution (e.g., `eval()`) is **FORBIDDEN**.
*   **Permissions:** Only the minimum necessary host permissions are requested.

### 4.2. Node.js API (Optional Backend)
*   **Input Sanitization:** **ALL** data received from any external source (including the extension for aggregated/anonymized telemetry) is sanitized using parameterized queries or ORM methods to prevent Injection attacks (SQL/NoSQL).
*   **Rate Limiting:** Aggressive rate limiting is implemented at API entry points to mitigate Denial of Service (DoS) and brute-force attacks.
*   **Secrets Management:** API keys and sensitive configuration are managed exclusively via environment variables (12-Factor App compliance) and are never checked into source control.

## 5. Automated Security Checks (CI/CD Integration)

Our continuous integration pipeline (`.github/workflows/ci.yml`) mandates the following security checks to run on every push:

1.  **Dependency Audit:** `npm audit` run with `--production` flag. Any High or Critical severity finding will fail the build.
2.  **Static Analysis:** Leveraging high-precision linters (TypeScript compiler strict checks) to catch type errors that often hide vulnerabilities.
3.  **SBOM Generation:** A Software Bill of Materials (SBOM) is generated during the build process for supply chain transparency.
4.  **Vulnerability Scanning:** Integration with GitHub Advanced Security features for dependency scanning.