# Security Policy

## Supported Versions

| Version | Supported | Description |
| :--- | :--- | :--- |
| `1.2.x` | Yes | Current stable release branch (`main`) |
| `< 1.2.0` | No | Legacy versions |

## Security and XSS Mitigation Scope

sleekeditor operates as a client-side rich-text editor processing user-supplied HTML. Security invariants include:
* **DOM-based XSS Defense**: All content passed to `setContent()` or produced by formatting routines must prevent script injection, event handler injection (`onerror`, `onload`), and untrusted URI schemes (`javascript:`, `data:` execution).
* **Zero Dependency Invariant**: sleekeditor must maintain zero third-party runtime dependencies to eliminate external supply-chain vulnerabilities.

## Reporting a Vulnerability

If you discover an XSS vulnerability, DOM injection vector, or sanitization bypass, please report it privately:

* **Security Contact**: Gohar Rehman
* **Email**: `goharrehmanfsd260@gmail.com`
* **Response SLA**: Initial acknowledgement within 48 hours; resolution timeline provided within 7 days.

Please do not open public GitHub issues or discussions regarding undisclosed vulnerabilities.