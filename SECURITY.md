# Security Policy

## Scope

Prompt Generator UI is a single-file, client-side application. There is no backend. Configurations are stored locally in the browser via localStorage.

## Reporting Vulnerabilities

- Please open an issue labeled `security` with a minimal, reproducible example.
- Do not include sensitive information. Provide steps and affected browser versions.
- Maintainers will triage and respond as soon as possible.

## Guidelines

- Avoid introducing external network calls or unsafe HTML rendering.
- Prefer `textContent` to prevent injection; avoid `innerHTML` unless strictly necessary and sanitized.
- Follow OWASP Top 10 principles; validate user-driven content before display.

## Disclosure

- Please do not publicly disclose details until a fix is available.
- After remediation, we will acknowledge the report in release notes or the relevant issue.
