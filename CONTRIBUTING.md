# Contributing to sleekeditor

Thank you for your interest in contributing to sleekeditor. We welcome contributions that improve cross-browser compatibility, formatting precision, and performance.

## Core Development Invariants
All contributions must adhere to our core project principles:
1. **Zero External Dependencies**: sleekeditor must never introduce external runtime dependencies, frameworks, or polyfill packages. All features must be implemented in clean Vanilla JavaScript.
2. **XSS Safety**: Any routine modifying DOM nodes or manipulating HTML strings must ensure inputs are sanitized and free from DOM-based XSS vulnerabilities.
3. **Cross-Browser Compatibility**: Features must work consistently across Chrome, Firefox, Safari, and Edge.

## Contribution Workflow
1. Fork and clone the repository:
   ```bash
   git clone https://github.com/<your-username>/sleekeditor.git
   cd sleekeditor
   ```
2. Create a focused branch:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Test locally by serving `index.html` via any static server.
4. Submit a Pull Request targeting `main`. Complete the mandatory security checklist in `.github/PULL_REQUEST_TEMPLATE.md`.