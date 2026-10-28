# Codex — implementation workflow for Stripe challenge

Use this only after the official Stripe brief has been converted into concrete requirements.

## First task for Codex

```text
You are working on a 48-hour hackathon project for the Stripe challenge.

First inspect the repository and summarize:
- current stack;
- how to run it locally;
- existing user flow;
- which parts are mocked;
- which parts are real;
- current Stripe integration, if any;
- obvious blockers or unsafe handling of credentials.

Do not rewrite the project or introduce a new framework unless necessary.

Then compare the current implementation against the official requirements in docs/PRODUCT_SPEC.md and produce the smallest implementation plan that closes the gaps.

Work in small, testable steps. For every change:
1. state the exact goal;
2. list files changed;
3. implement the minimum code;
4. give exact run/test commands;
5. describe one happy-path test and one failure-path test.

Rules:
- Stripe secret keys must stay server-side and out of Git.
- Use Stripe test/sandbox mode unless requirements explicitly say otherwise.
- Do not fake a Stripe success response and present it as real.
- Do not install major infrastructure without a concrete requirement.
- Prefer simple code the team can explain to judges.
- Preserve a working demo after every step.
```

## Later tasks

Once a real Stripe flow exists, use Codex for:

- fixing integration errors;
- webhook handling if required;
- validation and failure states;
- automated tests for the core scenario;
- setup instructions for teammates/judges;
- code cleanup shortly before submission.

Avoid giving Codex a giant request such as “build the whole hackathon project.” Small tasks are easier to verify and recover from.
