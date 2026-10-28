# Rapid user testing — hackathon version

Goal: test whether a person can **understand and use** the product without a teammate explaining it.

Do this repeatedly with people who did not design the feature. A 3–5 minute test is enough to reveal major problems.

## Test setup

Give the tester the app with no explanation beyond one sentence describing the scenario.

Do not tell them where to click. Do not explain terminology unless they are completely blocked. Observe first.

Record only anonymous notes unless the person explicitly agrees otherwise.

## Core questions

After the tester sees a result, ask:

1. **What do you think this screen is telling you?**
2. **What would you do next?**
3. **Which number or statement matters most here?**
4. **Why do you think the app gave you this result?**
5. **What, if anything, is unclear or makes you distrust the result?**

Do not ask “Do you like it?” first. That produces weak feedback.

## What to observe

Mark each item as PASS / ISSUE / BLOCKER.

- user understands the purpose of the screen in ~5 seconds;
- primary action is obvious;
- important financial terms are understood;
- user can distinguish inputs from assumptions;
- user understands whether a future value is a projection rather than a guarantee;
- user can find explanations without leaving the flow;
- user can recover from a wrong input;
- chatbot answer relates to the current screen/result;
- user can continue without knowing what an LLM, API or financial acronym is;
- mobile layout keeps the main takeaway visible.

## Chatbot test

Ask the tester to use natural language, including imperfect or vague wording.

Test prompts such as:

- “Nu înțeleg ce înseamnă asta.”
- “Explică-mi mai simplu.”
- “De ce ai ajuns la rezultatul ăsta?”
- “Ce se întâmplă dacă economisesc cu 300 lei mai puțin?”
- “Care este riscul?”

A good answer should:

- answer the actual question first;
- use context already on screen;
- avoid unnecessary jargon;
- not invent personal data;
- expose assumptions when relevant;
- give the user a concrete next action when useful.

## Voice test, if implemented

Test:

- noisy environment;
- Romanian amounts such as “trei mii cinci sute de lei”;
- dates;
- correction after wrong transcription;
- cancel/stop interaction;
- text alternative for every voice action.

Critical financial values should be confirmed visually before being used.

## Five-minute feedback format

For each tester, capture:

```text
Tester profile: [e.g. student / non-technical / financially experienced]
Task: [what we asked them to accomplish]
Completed without help: YES / NO
Main confusion:
Term they did not understand:
Action they expected but could not find:
Trust concern:
One thing to change immediately:
```

## Prioritisation rule

Fix problems in this order:

1. user cannot complete core flow;
2. user misunderstands financial meaning;
3. user does not trust or understand why a result appeared;
4. user cannot find next action;
5. cosmetic preference.

A visually imperfect screen that users understand is better than a polished screen that communicates the wrong thing.

## Demo readiness threshold

Before submission, the core flow should be tested by at least 3 people outside the immediate implementation work.

Target:

- 3/3 can complete the core task without verbal guidance;
- 3/3 can explain the main result in their own words;
- no tester mistakes a projection for a guaranteed outcome;
- no unexplained financial acronym blocks the flow;
- the most important action is found quickly.
