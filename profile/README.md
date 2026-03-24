# ⚓ KeelStack

### Build Your Next Startup, Not Just Boilerplate.

KeelStack delivers production-oriented, modular starter kits architected for the AI-assisted development era. We provide the essential, professional-grade plumbing — Auth, Payments, Security, Database — so you can focus on your unique idea and ship faster while owning all your code.

KeelStack focuses on providing well-structured starting points. Final quality, security, and compliance depend on how the system is configured, reviewed, and operated.

---

## What KeelStack Is — and Is Not

**KeelStack is:**
- Production-ready, opinionated starter systems for real SaaS businesses
- Built for founders who want full source ownership and long-term control
- Designed to work with AI coding tools, not fight them

**KeelStack is not:**
- A boilerplate zip dump
- A no-code or low-code platform
- A locked SaaS, hosted service, or vendor-controlled runtime
- A tutorial project or demo stack

---

## 🚀 Available Now

### KeelStack Engine — v1.1
*Node.js · Express · TypeScript · PostgreSQL · Stripe · Resend*

A production-grade backend foundation covering:
- Authentication — register, login, refresh tokens, MFA, password reset, email verification
- Billing — Stripe subscriptions, webhook handling, idempotency
- Background Jobs — async task queue, retryable job runner, persistent job store
- AI / LLM — provider-agnostic LLM client with per-user token budgets and boundary enforcement
- Database — PostgreSQL via Drizzle ORM with in-memory fallback
- Email — Resend integration
- Observability — Sentry and OpenTelemetry hooks
- Health endpoints — /healthz, /readyz, /health

**597 unit tests · 37 e2e checks · 93.13% statement coverage · 0 vulnerabilities**

Backend-only by design. Works with React, Next.js, Vue, Svelte, React Native, or any frontend you already have.

[Get KeelStack Engine →](https://keelstack.me)

---

### KeelStack UI Starter — v1.0 *(open source)*
*Next.js 14 · TypeScript · TanStack Query · Tailwind CSS*

A reference frontend that connects directly to the KeelStack Engine and demonstrates its production patterns in a working UI:
- Auth flows — login, register, MFA step, password reset, email verification (full token round-trip)
- Billing dashboard — subscription management with live idempotency key visibility and webhook deduplication demo
- Jobs dashboard — async task submission with 202 + poll lifecycle, real-time status tracking
- AI usage — token budget meter, LLMClient boundary explainer, per-call log

Not a generic dashboard. Every screen surfaces a specific engine pattern — idempotency keys, correlation IDs, 202+pollUrl flows, webhook dedup — so you can see exactly what the engine is doing and why.

[View on GitHub →](https://github.com/KeelStack-me/keelstack-ui-starter)

---

## 🗺️ Roadmap

These kits are in research or early design and will progress as the engine stabilises:

| Kit | Stack | Status |
|-----|-------|--------|
| Next.js Pro SaaS Starter | Next.js 15 · Drizzle · Tailwind · Stripe | Planned |
| AI Agent Kit | Python / Node · LangChain · OpenAI | Research |
| Mobile SaaS Starter | React Native · Expo · NativeWind | Research |

Roadmap items reflect current exploration and may change.

---

## ✨ Built for AI-Assisted Development

KeelStack is architected to work predictably with modern AI coding tools.

- `.cursorrules` included — curated context that reduces hallucinations and enforces architectural boundaries
- Deterministic structure — clear module boundaries so AI refactors don't break business logic
- Prompt-ready patterns — consistent, readable code that AI tools can safely extend

---

## Core Technology Choices

| Layer | Recommendation | Why |
|-------|---------------|-----|
| Payments | Stripe / Paddle | Global tax compliance, fraud protection, robust APIs |
| Authentication | Auth.js (v5) / Clerk | Edge-compatible, secure by default, framework agnostic |
| Database | PostgreSQL / Supabase | Relational integrity that scales from MVP to millions |
| Email | Resend / Postmark | Highest deliverability for transactional emails |

---

## 🛡️ Security & Trust

KeelStack takes a security-first approach to system design. Security depends on correct usage, configuration, and ongoing maintenance. KeelStack reduces common architectural mistakes — it does not eliminate risk entirely.

- Responsible vulnerability disclosure via private reporting channel
- Clear security boundaries and access control patterns
- Architected to support auditability and handling of real customer data

---

## 💬 Connect

- **Discussions:** [GitHub Discussions](https://github.com/orgs/KeelStack-me/discussions)
- **General:** [hello@keelstack.me](mailto:hello@keelstack.me)
- **Founder:** [founder@keelstack.me](mailto:founder@keelstack.me)
- **Support:** [support@keelstack.me](mailto:support@keelstack.me)
- **Security:** [security@keelstack.me](mailto:security@keelstack.me)
- **Website:** [keelstack.me](https://keelstack.me)

---

## 🤝 Community & Governance

- [Contributing Guidelines](https://github.com/KeelStack-me/.github/blob/main/CONTRIBUTING.md)
- [Security Policy](https://github.com/KeelStack-me/.github/blob/main/SECURITY.md)
- [Code of Conduct](https://github.com/KeelStack-me/.github/blob/main/CODE_OF_CONDUCT.md)

---

**Build fast. Stay secure. Own your code, data, and business — fully.** ⚓
