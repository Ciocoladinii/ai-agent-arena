# UX principles — make financial decisions understandable

Our UX responsibility is not only to make the app easy to operate. It must make the **financial meaning** of each output easy to understand for people with different levels of technical and financial literacy.

The Stripe brief explicitly values clarity, accessibility, intuitive interactions and a coherent end-to-end experience. Our design choices should therefore reduce confusion before adding more features.

## 1. Design for comprehension, not just navigation

Every important output should answer, in this order:

1. **What does this mean for me?**
2. **Why am I seeing this?**
3. **What assumptions were used?**
4. **What can I do next?**
5. **What should I be careful about?**

Avoid presenting a number, score or recommendation without context.

Bad:

> Risk score: 63/100

Better:

> Your plan is moderately sensitive to unexpected expenses. The main reason is that your emergency buffer covers less than two months of your current spending.

## 2. Plain Romanian first

Default to simple Romanian language. Financial terminology may be shown, but it should be translated into plain language immediately.

Example:

> **Volatilitate** — cât de mult poate varia valoarea unei investiții în timp.

Rules:

- short sentences;
- one idea per paragraph;
- avoid unexplained acronyms;
- prefer concrete examples in RON;
- explain percentages with an absolute-money example when useful;
- do not make the user feel unintelligent for not knowing a term.

## 3. Progressive disclosure

Do not show everything at once.

Default screen:

- key takeaway;
- 1–3 reasons;
- clear next action.

Optional details:

- assumptions;
- calculations;
- definitions;
- data sources;
- limitations;
- alternative scenarios.

Use controls such as `Why?`, `Show calculation`, `What does this mean?`, or `See assumptions`.

## 4. Outputs should be actionable

The app should not stop at information.

Each meaningful result should end with one or more concrete options, for example:

- change an assumption;
- compare a second scenario;
- set a target;
- save the plan;
- ask a follow-up question;
- view the calculation.

Avoid generic endings such as “Consider consulting a professional” as the only next step.

## 5. Make uncertainty visible

Financial outputs are often based on incomplete information, estimates or assumptions.

The UI should distinguish:

- **known input** — explicitly provided by the user;
- **assumption** — value estimated by the system;
- **projection** — calculated future scenario;
- **general information** — not personalised advice.

Never present a projection as guaranteed.

Useful wording:

> Based on the assumptions above...

> This is one possible scenario, not a prediction.

> We do not know X yet, so we assumed Y. You can change it here.

## 6. Chatbot is an interface, not the product

A chatbot may be used for text, voice or both, but the user should not be forced to discover the whole application through free-form chat.

Use the chatbot for:

- explaining results;
- asking clarifying questions;
- translating financial concepts into plain language;
- helping the user explore scenarios;
- answering follow-up questions about the current result.

Prefer structured UI for:

- important numbers;
- comparisons;
- assumptions;
- progress;
- actions;
- warnings.

A good pattern is:

`structured result → user asks question → chatbot explains → user can change inputs in UI`

The use of an LLM in the final product is **pending organiser/mentor confirmation**. The UX should remain coherent even if the conversational layer has to be replaced or reduced.

## 7. Voice interaction

If voice is included, voice should improve accessibility rather than exist as a novelty.

Requirements:

- show a text transcript;
- allow corrections before using important financial inputs;
- repeat critical amounts and dates visually;
- never require voice for core functionality;
- provide a clear way to stop/cancel listening;
- avoid reading long financial explanations aloud by default;
- ask for confirmation before accepting ambiguous numbers.

Example:

> I heard **3,500 RON per month**. Is that correct?

## 8. Accessible by default

Minimum expectations:

- readable font sizes;
- strong contrast;
- do not encode meaning only through colour;
- large click/tap targets;
- labels on icons;
- keyboard-friendly forms where possible;
- mobile layout that preserves the main takeaway;
- error messages next to the relevant input;
- avoid dense financial tables when a comparison card or chart communicates the same idea better.

## 9. Trust before persuasion

The interface should explain rather than pressure.

Avoid:

- artificial urgency;
- “best option” claims without criteria;
- hidden assumptions;
- exaggerated certainty;
- gamification that encourages risky financial behaviour.

Prefer:

- “why this result” explanations;
- visible assumptions;
- editable inputs;
- alternatives and trade-offs;
- explicit limitations.

## 10. Output template for core features

Whenever another teammate creates a new feature, try to map its result to this structure:

### Main result
One sentence understandable without financial knowledge.

### Why
Maximum 3 primary reasons.

### Numbers that matter
Only the numbers necessary to understand the decision.

### Assumptions
Editable where possible.

### Options
2–3 meaningful next actions or scenarios.

### Caveat
One short explanation of uncertainty, risk or limitation.

### Ask
The chatbot can explain any part of the result in simpler terms.

## UX definition of done

A feature is not done only because it works technically. It is done when a new user can:

- understand what the screen is about within ~5 seconds;
- identify the main result without asking a teammate;
- explain in their own words why they received that result;
- know what they can do next;
- distinguish facts from assumptions/projections;
- recover from an invalid or misunderstood input.
