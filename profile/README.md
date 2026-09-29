# ⚓ KeelStack

### Sponsor operations for solo newsletter and podcast creators.

KeelStack is a sponsor CRM and sponsor-facing portal for one-person newsletters and podcasts running 3–15 direct sponsorship deals. It replaces spreadsheets, email threads, and mental notes with a pipeline, a magic-link upload portal, automated renewal reminders, invoice tracking, and post-campaign performance reports.

**Website:** [keelstack.me](https://keelstack.me)

---

## What Lives Under This Name

Two separate things exist under the KeelStack name on GitHub. They are not the same product:

- **KeelStack** — a closed-source commercial platform. Sponsor operations for solo creators. This is what KeelStack is.
- **[Guard](https://github.com/KeelStack-me/guard)** — an open-source library we maintain. AI agent runtime safety. A standalone tool, unrelated to the sponsor product.

If you came here looking for Guard, skip to [Open Source](#open-source-guard). If you came here to find out what KeelStack is, it's sponsor operations.

---

## What KeelStack Is Today

**KeelStack is:**
- A sponsor CRM built for solo creators — not media teams, not ad-ops departments.
- A sponsor-facing portal where brands upload their own assets through a branded magic link. No account, no login.
- Platform-agnostic: works with Substack, Ghost, Kit, Mailchimp, Beehiiv (free/Scale tier), and any independent podcast host.

**KeelStack is not:**
- A sponsor marketplace or brand-matching network.
- A team-seat or ad-ops platform.
- A revenue-share tool — KeelStack takes 0% of your sponsorship revenue.

### What ships in the product

- **Sponsor pipeline** — Kanban stages: Pitched → Confirmed → Active → Renewed → Churned
- **Magic-link Sponsor Portal** — 24-hour, single-use, HMAC-hashed tokens. Sponsors upload logos, banners, ad copy, and tracking links, and see live deal status.
- **Renewal reminders** — automated 30/14/7-day sequence before contract end
- **Invoice tracking** — auto-generated invoices with a pending / paid / overdue dashboard
- **Performance reports** — CSV upload from any ESP, generating a branded one-page PDF summary per sponsor
- **Asset library** — every sponsor upload organized automatically per record
- **Revenue dashboard** — active sponsor MRR, per-sponsor breakdown, forward renewal calendar

Plans are $39/month (Starter), $59/month (Pro), and $99/month (Business). 14-day trial, no credit card required.

The product itself is **closed source**. It is not developed in public and there is no self-hosted distribution.

---

## Open Source: Guard

[Guard](https://github.com/KeelStack-me/guard) is an MIT-licensed runtime safety layer for AI agent workflows — idempotency gates, budget enforcement, and risk gating that prevent duplicate actions, budget overruns, and unsafe operations.

It predates KeelStack's move into creator tooling and continues to be maintained as a standalone library. It is **not** part of the sponsor product, and nothing in the sponsor product depends on it.

- Repository: [github.com/KeelStack-me/guard](https://github.com/KeelStack-me/guard)
- Package: [`@keelstack/guard`](https://www.npmjs.com/package/@keelstack/guard) on npm

Issues, questions, and contributions for Guard belong in the Guard repository — not in this org profile.

---

## Removed Repositories

**`keelstack-ui-starter`** was deleted in September 2026. It was a reference frontend for the former backend starter system. Any links to it are dead; it is not coming back.

**The backend engine** (KeelStack's original Node.js/TypeScript starter kit, March–April 2026) is discontinued. It was never published as a standalone repository and has no successor.

---

## Technology

The sponsor platform is closed source. Its stack, for those evaluating it:

| Layer | Used |
|---|---|
| Framework | Next.js (App Router) |
| Hosting | Vercel |
| Database | Neon Postgres via Prisma |
| File storage | Cloudflare R2 |
| Auth | Better Auth (creator accounts) + signed magic-link tokens (sponsors) |
| Email | Resend |
| Payments | Dodo Payments (Merchant of Record) |
| Analytics & errors | PostHog, Sentry |
| Scheduled jobs | Cloudflare Workers |

Guard has its own stack and dependencies, documented in [its repository](https://github.com/KeelStack-me/guard).

---

## Security & Trust

Security depends on correct configuration and ongoing maintenance. Current practices:

- Magic-link tokens are keyed-HMAC-hashed before storage. Raw tokens are never logged.
- Portal links are single-use, expire in 24 hours, and rotate any previously issued link and active session.
- Sponsor-facing sessions are separate, httpOnly, and time-limited. Sponsors never create an account.
- Billing webhooks are signature-verified and idempotent.
- Consent is versioned and auditable. Sponsor personal data flows through the Portal, so data export and deletion are built into the dashboard.

Responsible vulnerability disclosure is supported through the organization security policy. For Guard, use the repository's own security policy. For the sponsor platform, email below — please do not open public issues for security reports.

---

## Community & Governance

- [Security Policy](https://github.com/KeelStack-me/.github/blob/main/SECURITY.md)
- [Contributing Guidelines](https://github.com/KeelStack-me/.github/blob/main/CONTRIBUTING.md)
- [Code of Conduct](https://github.com/KeelStack-me/.github/blob/main/CODE_OF_CONDUCT.md)

The sponsor platform is closed source, so external contributions are limited to Guard. Questions about the product go to email, not GitHub.

---

## Connect

- Website: [keelstack.me](https://keelstack.me)
- General: [hello@keelstack.me](mailto:hello@keelstack.me)
- Security: [security@keelstack.me](mailto:security@keelstack.me)

---

**Give your sponsors a professional intake experience — and prove the campaign worked.** ⚓
