# Canonical Hackathon Brief — Stripe / VibeHack @ NEXXT Summit 2026

This file is the single source of truth for the challenge. Product decisions should be checked against it before implementation.

## Event

- Event: **VibeHack @ NEXXT Summit 2026**
- Dates: **28–29 October 2026**
- Track: **Stripe — Rethinking Financial Futures**

## Exact challenge

> **How can we make navigating the financial future a more accessible, relevant and empowering experience for people in Romania?**

### Your direction

The team chooses:

- the **audience**;
- the **financial need**;
- the **product experience** to address that need.

This means the challenge is deliberately broad. The product does **not** have to be a payments product, and the official slides do not require a Stripe API integration.

## What the final solution must demonstrate

The submission should clearly show:

1. **Who the product serves and which problem it solves.**
2. **How the core experience works end-to-end.**
3. **Why the solution is relevant in Romania.**
4. **Which assumptions, data sources, regulatory considerations and limitations apply.**

These four points are mandatory framing for both the product and the pitch.

## Stripe judging criteria

| Weight | Criterion | What it means |
|---|---|---|
| 20% | Challenge fit and differentiation | Romanian market fit, clear value proposition, what sets the product apart |
| 25% | User experience | Clear, accessible and intuitive end-to-end experience |
| 25% | Technical implementation | Execution quality, feasibility and a prototype that proves its value |
| 20% | Delivery and pitch | Clear story, strong demo and why the product matters |
| 10% | Business mentoring | Problem/user understanding, solution value and potential adoption |

### Practical consequence

UX + technical implementation = **50%** of the score. A small product that works well is preferable to a huge feature list that cannot be demonstrated reliably.

## Required deliverables and deadlines

### Wednesday, 28 October

- **14:00–15:30** — first checkpoint: approach and foundations ready.
- **18:30–20:00** — second checkpoint: first working MVP.
- **20:00** — pitch preparation workshop.
- After 20:00 — continue building and prepare demo/pitch.

### Thursday, 29 October

- **09:00** — ready to demonstrate and submit.
- **11:00 submission deadline**.
- Submission includes:
  - a **3-minute video pitch**;
  - **GitHub repository**;
  - **slide deck**.
- Three finalists are selected per challenge.
- Live finals are scheduled for **17:00**; each company jury picks its winner.

## Mentoring

### Stripe mentors

- Aleodor Tabarcea — Site Lead & Engineering Manager
- Bogdan Deac — Software Engineer
- Antonio Hus — Software Engineer
- George Chetreanu — Engineering Manager

### Mentoring model

- Technical mentoring is available throughout the hackathon for requirements, technical decisions and blockers.
- Business mentoring starts Thursday from 12:00 with two scheduled sessions focused on users, solution value and barriers to adoption.
- Mentor help is requested through Discord `#request-help`; team channels are private by default and mentors are invited when needed.

## Tools provided by the event

### Lovable

Lovable workshop and hackathon credits are provided. Use it primarily to accelerate UI/product development.

### Featherless AI

Featherless provides serverless inference for many open models through an **OpenAI-compatible API**. The event presentation shows the base URL:

`https://api.featherless.ai/v1`

The team already has an API key. **Never commit that key.** Store it only in local/cloud secrets, for example `FEATHERLESS_API_KEY`.

Featherless is an optional implementation tool. The Stripe challenge itself does not require an LLM or AI feature.

## What we must NOT assume

- Stripe Payments, Checkout, Connect, Billing or any other Stripe API is **not stated as mandatory** in the official slides.
- The solution is **not required to be an AI agent**.
- Featherless is **not required**; use it only if it materially improves the chosen user problem.
- We should not choose architecture before choosing the target user and financial problem.

## Current product status

**No product concept has been locked yet.**

The next decision is to choose one narrow Romanian audience + one meaningful financial problem + one end-to-end experience that can score well on challenge fit, UX, technical execution and demo quality.
