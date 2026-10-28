# Prompt inițial pentru Lovable

Create a polished, responsive hackathon MVP called **AI Agent Arena**. The product is a transparent interface where AI roles challenge an idea rather than simply agree with each other.

IMPORTANT: start with a **fully functional, explicitly labeled SIMULATED DEMO**, not fake API calls presented as real. No authentication, database, external integrations or API keys yet.

Build a single-page application with:
- A clear hero explaining “Challenge ideas. Expose assumptions. Improve reasoning.”
- A text area with an example prompt and a Start Arena button.
- Four readable sequential cards: (1) Proposer: initial answer and assumptions, (2) Challenger: concrete objections and counterexamples, (3) Proposer: revision, (4) Judge: balanced verdict, remaining uncertainties and next verification steps.
- Loading/progression UI, empty input validation, Reset, a copyable summary, and a compact “How it works” panel.
- A prominent badge reading “Simulated demo — no live AI calls” while simulated.
- Two or three selectable example scenarios; use deterministic canned responses for examples and label any generic placeholder output for custom prompts.
- Clean, accessible, mobile-first design with readable contrast and no distracting animations.
- A visible future integration boundary (document in code) for replacing simulated data with real server-side AI orchestration.

Acceptance criteria: works in preview, handles empty input, responsive on mobile, and does not imply the fake responses were generated live. Avoid complex dependencies. After building, tell me how to test each state and which files would need modification to connect a real LLM securely.
