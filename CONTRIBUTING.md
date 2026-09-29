# Contributing to KeelStack

First off, thank you for considering contributing to **KeelStack**.

KeelStack is an organization with two sides: a closed-source commercial product (a sponsor CRM for solo newsletter and podcast creators) and open-source community work.

**This guide applies only to public KeelStack repositories.** The KeelStack sponsor platform is closed source and does not accept external contributions. If you want to contribute to KeelStack, you contribute to Guard or to a future public project.

---

## Table of Contents
- [Code of Conduct](#code-of-conduct)
- [Where You Can Contribute](#where-you-can-contribute)
- [First Time? Start Here](#first-time-start-here)
- [How Can I Contribute?](#how-can-i-contribute)
- [Development Guidelines](#development-guidelines)
- [Pull Request Process](#pull-request-process)
- [Questions?](#questions)

---

## Code of Conduct

This project and everyone participating in it is governed by our [Code of Conduct](https://github.com/keelstack-me/.github/blob/main/CODE_OF_CONDUCT.md). By participating, you agree to uphold it.

Please report unacceptable behavior to [siddhant@keelstack.me](mailto:siddhant@keelstack.me), or [hello@keelstack.me](mailto:hello@keelstack.me) if your report concerns the founder. Full reporting process is in the Code of Conduct.

---

## Where You Can Contribute

| Repository | Status | Open to contributions? |
|---|---|---|
| [guard](https://github.com/KeelStack-me/guard) | Active | ✅ Yes |
| KeelStack sponsor platform | Closed source | ❌ No — no public repository exists |
| `keelstack-ui-starter` | Deleted Sept 2026 | ❌ No — repository no longer exists |

If a repository is not listed above as open, assume it is not open. Do not open pull requests against private repositories, and do not request that the sponsor platform be open-sourced.

---

## First Time? Start Here

New to open source or GitHub? We're glad you're here.

1. Explore issues labeled `good first issue` or `help wanted` in the relevant public repository.
2. Read the repository README and any linked docs before starting work.
3. Ask questions in the issue or discussion thread if anything is unclear.
4. You may use AI tools such as Copilot or Cursor to help draft code or docs, but you must review, understand, and test everything you submit.

---

## How Can I Contribute?

### AI Contributions Policy

We allow AI-assisted contributions, but the contributor remains fully responsible for the result.

- **Disclose meaningful AI use** in your PR description or commit message.
- **Understand your submission** and be able to explain what it does.
- **Test your changes** before submitting.
- **Do not submit low-quality or unreviewed AI-generated content.**

### Reporting Bugs

If you find a bug:

1. Search existing issues first.
2. Use the repository's bug template if one exists.
3. Include:
   - Environment details.
   - Clear steps to reproduce.
   - Expected vs actual behavior.
   - Relevant logs, screenshots, or error messages.
   - Severity and impact if known.

**Note:** This applies to public repositories only. Bugs in the KeelStack sponsor platform should be reported to [hello@keelstack.me](mailto:hello@keelstack.me), not as GitHub issues.

### Suggesting Features

If you have a feature idea:

1. Check the repository's Discussions or Ideas category first.
2. Explain:
   - The problem.
   - The proposed solution.
   - Why it fits the project.
3. Keep the suggestion focused and specific.

### Improving Documentation

Documentation contributions are welcome.

- Small fixes like typos or wording improvements can usually go straight to a PR.
- Larger changes should start with an issue or discussion first.

---

## Development Guidelines

### Code Style

- Follow existing patterns in the repository.
- Use clear names for variables, functions, and modules.
- Keep functions small and focused.
- Write code that is easy for humans and AI tools to read.
- Comment the **why**, not the obvious **what**.

### Commit Messages

We use [Conventional Commits](https://www.conventionalcommits.org).

Examples:
- `feat: add webhook retry handling`
- `fix: prevent duplicate token refresh`
- `docs: update installation instructions`
- `refactor: simplify guard evaluation`
- `test: add coverage for retry behavior`

### Review Expectations

All contributions are reviewed by a maintainer.

- Keep PRs small and focused.
- Be responsive to feedback.
- Expect some iteration before merge.
- Changes may be rejected if they do not fit the repository direction or quality bar.

---

## Pull Request Process

1. Fork the repository if needed.
2. Create a feature branch from `main`.
3. Make your changes.
4. Run tests and verify the repo still works.
5. Update docs if behavior changed.
6. Open a pull request.
7. Fill out the template clearly and explain the problem your change solves.

---

## Repository Scope

This contribution guide applies to **public community repositories** in the KeelStack organization — currently Guard, and any future open-source project published under this org.

The KeelStack sponsor platform is closed source. It has no public repository and does not accept external pull requests. This is a deliberate product decision, not an oversight, and it will not change.

---

## Questions?

- Community questions: use the repository discussions or Q&A area if available.
- Repo-specific issues: open an issue in the relevant public repository.
- Product or account questions (sponsor platform): [hello@keelstack.me](mailto:hello@keelstack.me)
- Security issues: follow the [Security Policy](https://github.com/keelstack-me/.github/blob/main/SECURITY.md).

Thank you for helping improve KeelStack.
