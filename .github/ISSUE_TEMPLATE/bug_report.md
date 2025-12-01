---
name: Bug Report
about: Report an issue with the AuraMind platform
title: '[BUG] Short, descriptive title'
labels: ['bug', 'triage']
projects:
  - 
assignees:
  - 
--- 

## 🐛 Summary of the Bug

Provide a concise, one-sentence summary of the observed behavior versus the expected behavior. 

*Example: When analyzing a session log, the sentiment score for 'frustration' sometimes resolves to `NaN` after the third API call.* 

---

## 🔬 Environment Details (Mandatory for Reproduction)

Adhere strictly to the Apex Technical Standards (Section 2.1 in `AGENTS.md`). Detail the specific context where the failure occurred.

### Platform Context

- **Extension Version:** (e.g., v1.2.0-alpha)
- **Browser:** (Chrome/Firefox/Edge version)
- **Operating System:** (e.g., macOS Sonoma 14.3, Windows 11)

### Backend Context (If applicable)

- **API Service Version:** (e.g., v0.9.1)
- **Node.js Version:** (Check with `node -v`)
- **Data State:** (e.g., Local Storage only, Connected to external PostgreSQL)

---

## 👣 Steps to Reproduce

Detail the exact, minimum steps required to trigger the bug. Treat this as a unit test case setup.

1. **Setup:** [Describe initial state, e.g., Logged into platform, opened settings panel.]
2. **Action 1:** [e.g., Navigate to the Session History dashboard.]
3. **Action 2:** [e.g., Click the 'Analyze All' button on the 5th session entry.]
4. **Observation:** [Describe what happened that was incorrect.]

---

## 💡 Expected Behavior

Describe what the system **should** have done according to the architectural blueprint and established principles (SOLID, DRY).

*Example: The platform should handle the `NaN` case by returning a default baseline sentiment score (0.0) or throwing a specific, non-crashing application error.* 

---

## 🚫 Actual Behavior

Describe exactly what happened. Include any relevant error codes, stack traces, or visual anomalies.


[Paste full console error/stack trace here]


If applicable, attach screenshots demonstrating the failure state, adhering to the UI/UX Aesthetic Singularity (Section 10 in `AGENTS.md`).

---

## 🔨 Potential Root Cause (Optional)

If you have identified a likely source (e.g., race condition, incorrect type casting, API timeout handling), document it here. Referencing section 8 (Reliability/Security) is encouraged.

*Example: Appears to be related to asynchronous data fetching in `src/features/telemetry/dataProcessor.ts` where the input validation guard clause is bypassed.* 
