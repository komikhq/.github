# Security Policy

KomikHQ takes the security and integrity of our digital infrastructure, edge services, and user data seriously. We appreciate the responsible disclosure of vulnerabilities by the security community.

---

## Supported Versions

We provide security updates for the current active release line (`main` branch) and latest production deployments:

| Project / Component | Supported | Notes |
| :--- | :--- | :--- |
| `komikhq/api` | Yes | Deployed edge endpoints and `main` branch |
| `komikhq/komikhq` | Yes | Production frontend releases and `main` branch |
| `komikhq/komikhq-clipper` | Yes | Latest extension build / stable branch |
| Legacy / Deprecated Archives | No | Historical reference only |

---

## Reporting a Vulnerability

**Please do not report security vulnerabilities via public GitHub issues, discussions, or pull requests.**

To report a vulnerability responsibly:

1. **GitHub Private Vulnerability Reporting**:
   - Where enabled, use the **Report a vulnerability** button under the **Security** tab of the respective repository.
2. **Direct Contact**:
   - Email our core team directly at **security@komikhq.com** (or reach out to organization administrators via GitHub profile contacts).

### What to Include in Your Report
- Detailed description of the vulnerability.
- Steps to reproduce the issue (including proof of concept scripts or curl commands where applicable).
- Potential impact and severity assessment.
- Affected components, endpoints, or repositories.

---

## Response Timelines and SLA

- **Acknowledgment**: Within 48 hours of report submission.
- **Triage and Assessment**: Within 5 business days.
- **Fix and Coordinated Disclosure**: Coordinated disclosure after resolution and production deployment.

We kindly ask that you keep information about the vulnerability confidential until a fix has been published and deployed to protect users and systems.
