# Lovable — workflow for Stripe: Rethinking Financial Futures

Use Lovable **after** the team selects a specific user, financial problem and end-to-end experience.

The official challenge does not require a Stripe API integration. Lovable should implement the chosen product experience, not invent the problem or force a payments flow.

## Before prompting Lovable

Fill these fields first:

- Target user in Romania: [USER]
- Financial problem: [PROBLEM]
- Desired outcome: [OUTCOME]
- Core user flow: [FLOW]
- Why this matters in Romania: [ROMANIAN RELEVANCE]
- Core logic/data source: [LOGIC / DATA]
- What is real: [REAL BEHAVIOUR]
- What is mocked/synthetic: [MOCKED DATA]
- Important limitation/edge case: [LIMITATION]
- Is AI actually needed? [YES/NO + WHY]

If these are unclear, do not start the full app yet.

## Prompt template

```text
Create a polished, responsive hackathon MVP for the Stripe challenge “Rethinking Financial Futures”.

Official challenge: make navigating the financial future more accessible, relevant and empowering for people in Romania.

Target user: [USER]
Specific financial problem: [PROBLEM]
Desired user outcome: [OUTCOME]
Why it matters in Romania: [ROMANIAN RELEVANCE]
Core end-to-end flow: [FLOW]
Core logic/data: [LOGIC / DATA]
Real behaviour that must work: [REAL BEHAVIOUR]
Mocked or synthetic data: [MOCKED DATA]
Important limitation/edge case: [LIMITATION]
AI usage: [NONE or EXACT AI FEATURE]

Optimize for the jury criteria:
- clear, accessible and intuitive UX;
- a working technical prototype that proves value;
- clear Romanian relevance and differentiation;
- a demo that can be explained in under 3 minutes.

Build only the minimum UI needed for the selected flow. Do not add authentication, payments, Stripe APIs, databases, AI features or dashboards unless they are explicitly part of the product definition above.

Clearly distinguish real calculations/API calls from mocked data. Add loading, success, error, empty and limitation states where relevant. Make the app mobile-friendly and visually coherent.

Never expose secret API keys in frontend code.

After building, explain:
1. which files were created or changed;
2. how to run and test the happy path;
3. how to test the failure/limitation path;
4. which parts are real and which are mocked;
5. any remaining technical risks before demo.
```

## Rule

The first Lovable version should prove the **user journey**, not maximize the number of screens.
