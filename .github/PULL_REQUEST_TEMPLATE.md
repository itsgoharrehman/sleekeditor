## Summary of Changes

Describe the proposed changes, API impact, and reason for the modification.

## Security and Quality Checklist

Before submitting this pull request, verify each of the following invariants:

- [ ] **Zero Runtime Dependencies**: Verified that no external npm or CDN dependencies are introduced.
- [ ] **XSS Sanitization**: Verified that formatting commands and HTML parsing routines do not introduce DOM-based XSS vectors.
- [ ] **Cross-Browser Tested**: Verified in at least two modern evergreen browsers (Chrome, Firefox, Safari, Edge).
- [ ] **Clean Code**: Verified Vanilla JS OOP standards and no console debugging logs left behind.

## Testing Performed

Detail the local tests or manual verification steps conducted in `index.html`.