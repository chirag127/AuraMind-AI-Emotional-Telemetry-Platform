# Security Policy

## Supported Versions

We are committed to maintaining the security of our platform. We actively support and patch the **latest stable release** of the AuraMind platform.

| Version | Supported          |
|---------|--------------------|
| Latest  | :white_check_mark: |

Older versions are not actively monitored for security vulnerabilities and are considered end-of-life.

## Reporting a Vulnerability

We take all security vulnerabilities seriously. If you discover a vulnerability in AuraMind, please report it to us as soon as possible through one of the following channels:

1.  **Email:** Send a detailed report to [security@auramind.io](mailto:security@auramind.io). Please use the subject line "Security Vulnerability Report - [Brief Description]".
2.  **GitHub Security Advisory:** Submit a private vulnerability report via [GitHub's security advisory feature](https://github.com/AuraMindAI/AuraMind-AI-Emotional-Telemetry-Platform/security/advisories/new).

**Please do NOT disclose any vulnerability publicly until it has been addressed.**

**When reporting a vulnerability, please include:**

*   A clear description of the vulnerability.
*   Steps to reproduce the vulnerability.
*   The affected version(s) of AuraMind.
*   Any potential impact or exploitability.
*   Proof of Concept (PoC) code, if available.
*   Your contact information.

## Vulnerability Disclosure Policy

*   **Responsible Disclosure:** We encourage you to follow responsible disclosure practices. Please give us a reasonable time to fix the issue before making any information public.
*   **No Harm:** Do not exploit any vulnerabilities you discover. This includes disrupting service, accessing or modifying data beyond what is necessary to confirm the vulnerability, or attempting to gain unauthorized access.
*   **Good Faith:** We will not pursue legal action against individuals who report vulnerabilities in good faith and adhere to this policy.
*   **Acknowledgement:** We will acknowledge receipt of your report promptly and will keep you informed of our progress in addressing the issue.

## Security Best Practices

As a platform for sensitive data, we adhere to the following security principles:

*   **Privacy-First Architecture:** Emotional telemetry data is processed locally by the browser extension whenever possible. Server-side processing is opt-in and anonymized.
*   **Zero Trust:** All external inputs are strictly validated and sanitized against OWASP Top 10 (2025) vulnerabilities.
*   **Data Encryption:** Sensitive data is encrypted both in transit (TLS/SSL) and at rest.
*   **Dependency Auditing:** We regularly audit third-party dependencies for known vulnerabilities using automated tools.
*   **Secure Development Lifecycle (SDL):** Security is integrated into every phase of development, from design to deployment.
*   **Least Privilege:** Components and services operate with the minimum necessary permissions.
*   **Rate Limiting:** The optional Node.js API is protected by robust rate limiting to prevent abuse.

## Security Contact

For general security inquiries or to discuss security-related matters that do not involve reporting a specific vulnerability, please contact [security@auramind.io](mailto:security@auramind.io).
