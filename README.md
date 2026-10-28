# Stripe — Rethinking Financial Futures | VibeHack @ NEXXT Summit 2026

This repository is the working space for our **Stripe challenge**.

## Official challenge

> **How can we make navigating the financial future a more accessible, relevant and empowering experience for people in Romania?**

We choose the:

- **audience**;
- **financial need**;
- **product experience**.

The product must clearly demonstrate:

1. who it serves and what problem it solves;
2. how the core experience works end-to-end;
3. why it matters in Romania;
4. assumptions, data sources, regulatory considerations and limitations.

## Judging

- **25%** User experience
- **25%** Technical implementation
- **20%** Challenge fit and differentiation
- **20%** Delivery and pitch
- **10%** Business mentoring

## Current product direction

The team is exploring an application with a conversational layer (text, voice or both) alongside structured financial outputs. The final AI usage still needs confirmation from organisers/mentors; QA DNA has an explicit no-LLM final-system rule, while no equivalent restriction appears in the official Stripe materials we have.

The UX focus is broader than making the app easy to operate: financial outputs must be understandable to users with different levels of technical and financial literacy.

## Start here

1. [Canonical hackathon brief](docs/HACKATHON_BRIEF.md)
2. [Immediate next steps](docs/START_HERE.md)
3. [Product specification / concept selection](docs/PRODUCT_SPEC.md)
4. [UX principles for financial comprehension](docs/UX_PRINCIPLES.md)
5. [Rapid user testing checklist](docs/USER_TESTING.md)
6. [Available tools and Featherless setup](docs/TOOLS.md)
7. [Lovable workflow](docs/LOVABLE_PROMPT.md)
8. [Codex workflow](docs/CODEX_PROMPT.md)
9. [Team playbook](docs/TEAM_PLAYBOOK.md)

## Critical clarification

The official brief does **not** require Stripe Payments, Checkout, Connect, Billing or another Stripe API integration. Stripe is the challenge sponsor; technology should follow the chosen problem.

AI is a possible implementation tool, not the value proposition by itself. Featherless credits/API access are available, but an LLM should only be used if it materially improves the user experience or core functionality.

## Event deadlines

Wednesday 28 October:

- 14:00–15:30 — approach and foundations checkpoint
- 18:30–20:00 — first working MVP checkpoint
- 20:00 — pitch preparation workshop

Thursday 29 October:

- 09:00 — ready to demonstrate and submit
- 11:00 — submission deadline
- Submission: **3-minute video pitch + GitHub repository + slide deck**
- 17:00 — live finals

## Tooling available

- **Lovable** — connected by the team, hackathon credits available.
- **Featherless AI** — team API key available; OpenAI-compatible endpoint shown by organisers.
- **ChatGPT / Codex** — planning, implementation, debugging, testing and documentation.
- **GitHub** — source of truth for code and project documentation.

## Security

Never commit API keys, `.env` files or credentials. The Featherless key must remain in environment/secret storage only.

## Repository name

Recommended final name: **`vibehack-stripe-2026`**.

If this repository is still named `ai-agent-arena`, rename it in GitHub:

`Settings → General → Repository name → vibehack-stripe-2026 → Rename`
