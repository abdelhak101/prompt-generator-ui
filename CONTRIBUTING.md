# Contributing

Thank you for your interest in contributing to Prompt Generator UI. This project is a single-file, client-side tool designed to help think through UI/UX and generate structured prompts.

## Workspace

- Open: [prompt-generator.html](/prompt-generator.html) in a modern browser (Edge/Chrome/Firefox/Safari).
- No build or server required; all state is stored locally in your browser.
- Test both Dark and Light themes and verify Copy/Download/Export/Import functions.

## Getting Started

- Fork the repository.
- Create a feature branch: `feat/<short-name>` or `fix/<short-name>`.
- Make changes and validate locally by opening the HTML file.
- Push and open a Pull Request with a clear summary and screenshots (if UI changes).

## Design & UX Guidelines

- Follow the checklists in [README](/README.md) (visual hierarchy, cognitive load, readability, consistency, accessibility, responsiveness).
- Ensure WCAG 2.1 AA contrast and keyboard focus states remain intact.
- Keep interactions subtle; avoid distracting motion unless explicitly configured.

## Coding Guidelines

- Keep the app dependency-free and client-side only; do not introduce external network calls.
- Use semantic HTML and accessible controls; preserve aria attributes in accordions and buttons.
- JavaScript should remain modular and side-effect aware; avoid global leaks.
- Do not store or process sensitive/PII data; configurations remain in localStorage.

## Security & Compliance

- Avoid introducing vulnerabilities per OWASP Top 10 (e.g., XSS via unescaped user content).
- Validate/sanitize any content that could be rendered; prefer textContent over innerHTML.
- See [SECURITY.md](/SECURITY.md) for reporting.

## Commit Messages

- Use Conventional Commits:
  - `feat: add new preset loader`
  - `fix: correct accordion aria-expanded`
  - `docs: update README usage`
  - `refactor: simplify updatePrompt sections`
  - `chore: tidy formatting`

## Pull Request Checklist

- Description of change and motivation.
- Screenshots/GIFs for UI updates.
- Cross-browser manual checks (Edge, Chrome).
- Accessibility checks (tab order, focus indicators, contrast).
- Security checks (no external calls, no unsafe HTML rendering).
- Documentation updates if behavior changes.

## Issues

- Bug reports: use the Bug Report template and include steps, expected/actual behavior, and environment.
- Feature requests: describe the problem, proposed solution, alternatives, and impact.

## Code of Conduct

- Be respectful and constructive. See [CODE_OF_CONDUCT.md](/CODE_OF_CONDUCT.md).

## License

- By contributing, you agree your contributions are licensed under the project’s [MIT License](/LICENSE).
