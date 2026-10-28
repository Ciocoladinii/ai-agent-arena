# Stripe Challenge — VibeHack / NEXT AI Hackathon 2026

This repository is now the working space for our **Stripe challenge** at the hackathon.

> Previous direction: QA DNA / AI Agent Arena. That direction is abandoned and should not guide implementation.

## Current status

We have been assigned to **Stripe**, but we do not yet have the full official Stripe brief in this repository. Until the brief arrives, we do **not** build product-specific features or invent requirements.

Our immediate goal is to be ready to move fast once the official materials arrive.

## Working principles

- Build the smallest end-to-end demo that satisfies the official brief.
- Heavy use of ChatGPT, Codex and Lovable for vibe coding is expected.
- Prefer simple, understandable architecture over impressive but fragile complexity.
- Keep one main repository and small feature branches when multiple people start coding.
- Test every generated change before merging it.
- Never commit secrets, Stripe keys, `.env` files or credentials.
- Use Stripe test/sandbox tooling unless the official challenge explicitly requires something else.
- Do not add infrastructure (Docker, databases, queues, extra services) without a concrete need.

## Start here

- [Immediate checklist](docs/START_HERE.md)
- [Stripe brief intake / requirements](docs/PRODUCT_SPEC.md)
- [Lovable instructions](docs/LOVABLE_PROMPT.md)
- [Codex instructions](docs/CODEX_PROMPT.md)
- [Team playbook](docs/TEAM_PLAYBOOK.md)

## Repository rename

Recommended repository name: **`vibehack-stripe-2026`**.

The connected GitHub tool can edit repository contents but cannot rename the repository itself. Rename it in GitHub via:

`Repository → Settings → General → Repository name → vibehack-stripe-2026 → Rename`

GitHub normally redirects the old repository URL after a rename, so existing local clones can still be repaired easily if needed.

## Important

Do not start a Lovable build from the old AI Agent Arena prompt. The old product concept is no longer relevant.
