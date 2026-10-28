# Codex — implementation workflow for Stripe: Rethinking Financial Futures

Use this after the team has selected a concrete user, financial problem and core flow.

The official challenge does **not** require a Stripe API integration. Codex should implement the chosen product and preserve a working demo, not force a payments architecture.

## First task for Codex

```text
You are working on a 48-hour hackathon project for the Stripe track “Rethinking Financial Futures”.

Official challenge: make navigating the financial future more accessible, relevant and empowering for people in Romania.

First inspect the repository and summarize:
- current stack;
- how to run it locally;
- existing user flow;
- which parts are mocked versus real;
- current data/AI/API integrations;
- obvious blockers, unsafe credential handling, or architecture risks.

Then read docs/HACKATHON_BRIEF.md and docs/PRODUCT_SPEC.md and compare the implementation against the chosen product definition.

Do not rewrite the project or introduce a new framework unless necessary.

Work in small, testable steps. For every change:
1. state the exact goal;
2. list files changed;
3. implement the minimum code;
4. give exact run/test commands;
5. describe one happy-path test and one failure/limitation test;
6. state what is real and what is mocked.

Rules:
- Preserve a working demo after every step.
- Never print or commit secrets.
- Keep Featherless or any other API keys server-side / in secret storage.
- Do not add Stripe APIs unless the chosen product actually needs them.
- Do not add AI merely because Featherless credits are available.
- Do not install major infrastructure without a concrete requirement.
- Prefer code the team can understand and explain to judges.
- Optimize for the jury criteria: UX, technical quality, challenge fit, and demo clarity.
```

## Good Codex tasks

- implement one screen or user-flow step;
- wire one calculation or API call;
- fix one integration error;
- add loading/error/limitation states;
- add tests for the core scenario;
- review security/secrets handling;
- make setup reproducible;
- clean up code before submission.

Avoid requests like “build the entire hackathon project”. Small tasks are easier to test, explain and recover from.
