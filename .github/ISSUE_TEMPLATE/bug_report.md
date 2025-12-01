---
name: Bug Report
about: Report a bug or unexpected behavior in the AuraMind platform.
title: "Bug: [Concise description of the issue]"
labels: bug
assignees: ""

body:
  - type: markdown
    attributes:
      value: | # THE BUG REPORT PROTOCOL (DECEMBER 2025 EDITION)
        Thank you for reporting an issue with the **AuraMind AI Emotional Telemetry Platform**! Please provide as much detail as possible to help us diagnose and resolve the problem swiftly.

        **Severity Levels:**
        *   **Critical:** System down, major data loss, security breach.
        *   **High:** Core functionality broken, significant degradation.
        *   **Medium:** Minor functionality broken, moderate degradation.
        *   **Low:** UI glitches, documentation errors, minor inconveniences.

        --- #

  - type: dropdown
    id: severity
    attributes:
      label: Severity Level
      description: Choose the severity level that best describes this bug.
      options:
        - Critical
        - High
        - Medium
        - Low
      isMultiple: false
    validations:
      required: true

  - type: input
    id: affected-component
    attributes:
      label: Affected Component(s)
      description: Which part of the platform is experiencing this issue? (e.g., Browser Extension, Node.js API, Web UI, Data Visualization).
      placeholder: "Browser Extension, Node.js API, Web UI, etc."
    validations:
      required: true

  - type: textarea
    id: description
    attributes:
      label: Detailed Description
      description: Provide a clear and concise explanation of the bug. What did you expect to happen, and what actually happened?
      placeholder: |-
        Describe the observed behavior and the expected behavior.
        Example:
        *Expected:* When I click the 'Export Data' button, a CSV file should be generated and downloaded.
        *Actual:* Clicking the 'Export Data' button results in a '500 Internal Server Error' message in the browser console, and no file is downloaded.
    validations:
      required: true

  - type: textarea
    id: steps-to-reproduce
    attributes:
      label: Steps to Reproduce
      description: Provide a step-by-step guide on how to reproduce the bug. Be as specific as possible.
      placeholder: |-
        1. Navigate to the 'Dashboard' page.
        2. Ensure the 'Real-time Mode' is enabled.
        3. Perform action X.
        4. Observe error Y.
    validations:
      required: true

  - type: textarea
    id: environment-details
    attributes:
      label: Environment Details
      description: Specify the environment in which the bug occurred.
      placeholder: |-
        *   **Operating System:** (e.g., Windows 11, macOS Sonoma 14.2, Ubuntu 23.10)
        *   **Browser (if applicable):** (e.g., Chrome 120.0.6099.109, Firefox 115.0.2)
        *   **Browser Extension Version (if applicable):** (e.g., v1.2.3)
        *   **Node.js Version (if applicable):** (e.g., v20.10.0)
        *   **API Endpoint (if applicable):** (e.g., `/api/v1/telemetry`)
        *   **Any relevant configurations or settings.**
    validations:
      required: true

  - type: textarea
    id: logs-and-screenshots
    attributes:
      label: Logs and Screenshots (Optional but Recommended)
      description: Attach any relevant console logs, error messages, screenshots, or screen recordings that can help illustrate the problem.
      placeholder: |-
        *   **Console Logs:** Paste any relevant error messages from the browser's developer console or the Node.js server logs.
        *   **Screenshots:** Upload screenshots highlighting the issue.
        *   **Screen Recordings:** Link to a screen recording (e.g., Loom, YouTube).
    validations:
      required: false

  - type: textarea
    id: additional-context
    attributes:
      label: Additional Context
      description: Provide any other information that might be relevant to the bug.
      placeholder: |-
        This bug seems to only occur when...
        I noticed this behavior after updating...
    validations:
      required: false

---
