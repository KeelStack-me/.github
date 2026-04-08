# 🛡️ KeelStack Security Policy

At **KeelStack**, we are committed to building secure **AI‑Native SaaS Starter Kits** for solo founders and indie hackers. This policy applies to **all repositories** within the KeelStack organization, including our public community repos and private template repos.

We welcome the efforts of security researchers to help us maintain the highest level of integrity for our customers and our code. This policy is designed to be clear, fair, and actionable.

---

## 🔒 Supported Versions

We actively maintain and provide security updates only for the **latest major version** of each KeelStack product.

| Version | Supported |
| :--- | :--- |
| Latest major version | ✅ |
| Older major versions | ❌ |

Users are strongly encouraged to keep their installations up to date. Security fixes are **not backported** to unsupported versions.

---

## 📢 Reporting a Vulnerability

If you discover a security vulnerability in any KeelStack repository, **please do not open a public issue**. Public disclosure before a fix is available puts our users at risk.

Instead, report all security concerns through one of the following private channels:

- **GitHub Private Vulnerability Reporting** (recommended): Go to the **Security** tab of the relevant repository and click **Report a vulnerability**.
- **Email**: [security@keelstack.me](mailto:security@keelstack.me).

Reports are handled privately and access is restricted to core maintainers.

---

## ⏱️ What to Expect

We follow a **Coordinated Vulnerability Disclosure (CVD)** process. You can expect:

| Step | Timeline |
| :--- | :--- |
| **Acknowledgement** | Within 24 hours (often sooner) |
| **Triage & Confirmation** | Within 5 business days |
| **Status updates** | Weekly throughout the investigation |
| **Fix & release** | Within 90 days (typical) |

If we cannot resolve the vulnerability within 90 days, we will work with you to establish a revised disclosure timeline or acknowledge your right to public disclosure.

We will keep you informed of our progress and may request additional information. The Red Hat Product Security team follows a similar process, acknowledging reports within one business day.

---

## 🛠️ Disclosure Policy

We follow **Coordinated Vulnerability Disclosure**. We ask that you allow us a reasonable amount of time to resolve the issue before making any public disclosure. We will work with you to agree on a disclosure timeline.

### ✅ In Scope

Vulnerabilities in the following areas are considered in scope:

- Authentication bypass (e.g., Auth.js, JWT logic, session management)
- Data leakage (API endpoints, middleware, environment variables)
- Injection flaws (SQL, NoSQL, command injection)
- Insecure configuration (deployment scripts, Docker settings, Cloudflare rules)
- Broken access control (RBAC, user permissions, tenant isolation)
- Remote code execution (RCE)

**Note:** Security reports for **custom implementations** built using KeelStack are out of scope; we only cover the **Core Template logic** (authentication, authorization, billing, webhook handling, and infrastructure scaffolding).

### ❌ Out of Scope

- Issues in third‑party dependencies (please report to the respective maintainers)
- Theoretical attacks without a proof‑of‑concept
- Social engineering, phishing, or physical attacks
- Denial‑of‑service (DoS) attacks
- Automated tooling reports without manual verification
- Reports from automated scanners that lack demonstrated impact

---

## 🔐 Safe Harbor

We will not pursue legal action against security researchers who discover and report vulnerabilities **responsibly and in good faith**, in accordance with this policy. We consider the following activities as authorised:

- Conducting research on KeelStack products without causing harm
- Testing in accordance with this policy
- Making a good‑faith effort to avoid privacy violations, destruction of data, or interruption of service

We ask that you:

- **Do not** access, modify, delete, or exfiltrate data beyond what is strictly necessary to demonstrate the vulnerability
- **Do not** perform denial‑of‑service attacks or degrade system availability
- **Do not** introduce malware, backdoors, or malicious code
- **Do not** perform social engineering attacks
- **Do not** disclose the vulnerability publicly before we have had a reasonable opportunity to investigate and remediate it

---

## 🤝 Acknowledgments

We believe in giving credit where it’s due. If you are the **first** to report a unique, valid security issue, we will:

- Give you **public credit** in our release notes (unless you prefer to remain anonymous)
- Grant you a **complimentary Premium License** (scope and duration determined at our discretion) to our latest SaaS Starter Kits

We do not currently operate a bug bounty program, but we deeply appreciate every contribution that makes KeelStack more secure.

---

## 🧭 Threat Model & Security Hardening

KeelStack is designed with security in mind. We follow industry best practices:

- **Input validation** using Zod schemas
- **Rate limiting** on authentication endpoints (30 requests / 10 minutes)
- **Helmet.js** for secure HTTP headers (strict CSP, HSTS, no sniff)
- **Argon2id** for password hashing (OWASP 2023 parameters)
- **Constant‑time comparison** for sensitive operations
- **Idempotency middleware** to prevent duplicate webhook processing
- **Durable job queues** with retry‑safe execution
- **Environment‑based configuration** with `.env.example` – never commit secrets

For more details, refer to our [Security Hardening Guide](./docs/SECURITY.md) and the **Security** section in our documentation.

---

Thank you for helping us keep KeelStack and the indie hacking community safe. Together, we build better.

– **The KeelStack Team ⚓**
