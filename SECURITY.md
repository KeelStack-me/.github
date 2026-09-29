# KeelStack Security Policy

At KeelStack, we take security seriously across everything we operate — our open-source repositories and our closed-source sponsor platform alike.

This policy applies to all KeelStack-maintained code and services unless a more specific repository-level or service-level security policy is provided. Two surfaces are covered: **public repositories** (currently [Guard](https://github.com/KeelStack-me/guard)) and the **KeelStack sponsor platform** (`keelstack.me` / `app.keelstack.me`).

We welcome security researchers and community members who help us improve the security of KeelStack software. This policy is designed to make responsible reporting clear, private, and actionable.

---

## Supported Versions

We actively maintain and provide security updates only for the latest major version of each KeelStack product or repository line.

| Version | Supported |
| :--- | :--- |
| Latest major version | ✅ |
| Older major versions | ❌ |

Security fixes are not backported to unsupported versions unless explicitly stated in a repository-specific policy or release announcement.

---

## Reporting a Vulnerability

Please do not open a public issue for a security vulnerability, and do not disclose it publicly before we've had a chance to investigate.

**Public repositories (e.g. Guard)** — use **GitHub Private Vulnerability Reporting**: open the **Security** tab of the affected repository and select **Report a vulnerability**. If that isn't enabled on the repository, use the email below.

**KeelStack sponsor platform** (`keelstack.me`, `app.keelstack.me`) — email [security@keelstack.me](mailto:security@keelstack.me). There is no public repository for the platform, so email is the only private channel.

Please include, if possible:
- A clear description of the issue.
- The affected repository or service, and version if applicable.
- Steps to reproduce.
- The security impact.
- Any proof of concept or relevant logs, if safe to share.

---

## Coordinated Disclosure

We follow a Coordinated Vulnerability Disclosure process.

| Step | Timeline |
| :--- | :--- |
| Acknowledgement | Within 24 hours |
| Triage and confirmation | Within 5 business days |
| Status updates | Weekly during investigation |
| Fix and release | Typically within 90 days |

If we cannot resolve the issue within 90 days, we will work with the reporter to agree on a revised disclosure timeline. If necessary, we will also discuss whether public disclosure should proceed.

---

## Safe Harbor

We will not pursue legal action against researchers who report vulnerabilities responsibly and in good faith, in accordance with this policy.

Authorized research includes:
- Testing KeelStack repositories and the sponsor platform for security issues.
- Reviewing public repository code and configuration.
- Validating a vulnerability with the minimum proof needed to demonstrate impact.
- Coordinating privately with maintainers before public disclosure.

Please do not:
- Access, modify, delete, or exfiltrate data beyond what is necessary to demonstrate the issue.
- Perform denial-of-service attacks or degrade service availability.
- Introduce malware, backdoors, or malicious code.
- Use social engineering or phishing.
- Publicly disclose the vulnerability before we have had a reasonable opportunity to investigate and remediate it.

---

## Scope

### In Scope

Security issues are in scope when they affect KeelStack-maintained code or services.

**Public repositories (Guard):** reports may be based on reading the source. Relevant areas include authentication and authorization logic, injection flaws, unsafe defaults, dependency handling, and anything shipped as part of the library.

**Sponsor platform (black-box testing only — source is not public):** relevant areas include magic-link token handling and portal session security, creator authentication and account access control, cross-account data exposure, file upload and asset storage handling, billing and subscription webhook verification, consent and personal-data handling, and API authorization.

In both cases: insecure configuration, secrets exposure, and signed-webhook bypasses are in scope.

### Out of Scope

The following are out of scope:
- Vulnerabilities in third-party dependencies, unless caused by KeelStack integration code.
- Theoretical attacks without a proof of concept.
- Social engineering, phishing, or physical attacks.
- Denial-of-service attacks that do not demonstrate a security impact.
- Automated scanner reports without manual verification and impact.
- Issues in custom implementations built by users on top of KeelStack code unless the issue is caused by KeelStack-provided code.
- Attempts to access another user's account or data beyond the minimum needed to demonstrate a vulnerability.

---

## What to Expect

We aim to handle reports professionally and transparently.

- We may request additional information or clarification.
- We may ask you not to disclose the issue publicly until a fix is available.
- We may coordinate on a temporary mitigation if a full fix will take time.
- We may publish a security advisory after the fix is released.

If you prefer anonymity, please let us know and we will respect that where possible.

---

## Acknowledgments

If you are the first to report a unique, valid security issue, we may credit you in release notes or advisories, unless you prefer to remain anonymous.

We do not currently operate a formal bug bounty program and do not offer monetary rewards.

---

## Security Hardening

KeelStack repositories and services should use security best practices appropriate to the project, including:
- Input validation.
- Secret scanning and push protection.
- Dependency review and updates.
- Secure defaults.
- Environment-based configuration.
- Signed webhooks where applicable.
- Rate limiting where implemented.
- Audit logging where applicable.

For repository-specific guidance, see that repository's documentation.

---

## Contact

- Security reports: [security@keelstack.me](mailto:security@keelstack.me)
- General and product questions: [hello@keelstack.me](mailto:hello@keelstack.me)
