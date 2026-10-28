# Team playbook — Stripe challenge / 48h vibe coding

## Core rule

We optimize for a **working, explainable, testable demo**, not for maximum technical complexity.

## Before coding

Everyone should understand:

- the official Stripe challenge statement;
- the core user;
- the minimum scenario the jury must be able to test;
- which Stripe product/API is actually required;
- what can be mocked and what must be real;
- judging criteria and demo format.

If the team cannot explain those points in one minute, implementation starts too early.

## Team roles when people arrive

### 1. Product / brief owner
- turns the official brief into concrete acceptance criteria;
- keeps the team aligned with jury criteria;
- prepares the demo story and pitch.

### 2. UI / flow owner
- builds the minimum interface;
- handles loading, success, failure and edge cases;
- keeps the demo readable and fast.

### 3. Stripe integration owner
- implements the real Stripe test-mode interaction;
- protects keys and secrets;
- understands request/response flow well enough to explain it.

### 4. Integration / QA owner
- runs the project from a clean setup;
- tests happy path and failure path;
- reviews generated AI code before merge;
- keeps README/setup steps current.

With 2–3 people, combine roles. Do not wait for the full team before making progress.

## Vibe coding rules

- Give ChatGPT/Codex/Lovable small, precise tasks.
- Never merge generated code just because it looks plausible.
- After every meaningful change, run the app and test it manually.
- Ask the coding agent to state exactly which files changed and how to test them.
- Keep changes reversible and commit frequently.
- One teammate should own integration/merges once concurrent work starts.

## Development sequence

1. Parse official brief and jury criteria.
2. Define one end-to-end user flow.
3. Build a minimal deterministic UI shell.
4. Implement the smallest real Stripe test-mode interaction required.
5. Add one meaningful failure/edge case.
6. Make setup reproducible on another laptop.
7. Improve UX only after the core works.
8. Add optional differentiators only if the demo remains stable.
9. Freeze features before judging and rehearse the demo.

## Branch strategy

- `main` should remain runnable.
- Use short feature branches once multiple teammates code simultaneously.
- Keep PRs small enough that another teammate can review them quickly.
- Avoid multiple people modifying the same core file at the same time when possible.

## Infrastructure

Do not use a second laptop as a home server by default. GitHub, Lovable, Codex and normal cloud deployment are enough for initial development. A second laptop becomes useful only for a specific reason such as cross-device testing or running a local service required by the chosen architecture.

## Security

- Never commit Stripe secret keys.
- Never paste secrets in screenshots, prompts, issues or README files.
- Use `.env` locally and only commit `.env.example` without real values.
- Use Stripe test/sandbox credentials during development unless official requirements state otherwise.
- Do not expose server-side keys to frontend JavaScript.

## Final demo checklist

- Fresh browser session works.
- Core scenario works from start to finish.
- Failure path is handled cleanly.
- Team can explain what is real versus mocked.
- Stripe integration can be explained without hand-waving.
- README setup instructions work on a teammate's machine.
- No secrets exist in Git history or frontend code.
