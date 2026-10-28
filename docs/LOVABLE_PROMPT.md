# Lovable — use only after the Stripe brief is understood

Do **not** paste a product prompt into Lovable before we understand the official Stripe challenge.

## When the brief arrives

Use Lovable for the visual shell and user flow, not for inventing requirements.

Before prompting Lovable, define:

- target user;
- core problem;
- exact happy-path flow;
- one important failure/edge case;
- what Stripe interaction is real;
- what data is mocked;
- what the jury must be able to verify.

## Prompt template

Replace every [PLACEHOLDER] before use.

```text
Create a polished, responsive hackathon MVP for the Stripe challenge.

Problem: [EXACT PROBLEM]
Target user: [USER]
Core user flow: [STEP-BY-STEP FLOW]
Stripe capability used: [STRIPE PRODUCT/API]
Required real behavior: [WHAT MUST ACTUALLY WORK]
Allowed mocked data: [WHAT CAN BE SIMULATED]
Important edge case: [FAILURE/EDGE CASE]

Build only the minimum UI needed for this flow. Keep the architecture simple and easy to modify during a hackathon. Do not add login, payments, a database, AI features, dashboards or integrations unless they are explicitly required above.

Never put Stripe secret keys in browser code. Clearly separate UI mock data from real Stripe test-mode interactions. Add useful loading, success and error states. Make the app mobile-friendly and easy to demo in under 90 seconds.

After building, explain:
1. which files were created;
2. how to test the happy path;
3. how to test the failure path;
4. what still uses mock data;
5. what is needed for the real Stripe integration.
```

## Rule

If we cannot fill the placeholders from the official brief, we are not ready to generate the app yet.
