# Hackathon Tools — Lovable, Featherless, ChatGPT/Codex

## Lovable

Status: **connected / credits available**.

Use Lovable to accelerate the user-facing product experience once the product concept is chosen. It should not invent the business problem for us.

Recommended use:

- build the first responsive UI shell;
- iterate quickly on the core user flow;
- add loading/error/empty states;
- prepare a polished demo path;
- keep generated code simple enough for the team to understand.

Do not add authentication, databases or third-party services unless the chosen flow requires them.

## Featherless AI

Status: **API key available to the team**.

Featherless provides OpenAI-compatible access to open models.

Base URL shown in the event materials:

`https://api.featherless.ai/v1`

Environment variable convention:

```bash
FEATHERLESS_API_KEY=your_key_here
FEATHERLESS_BASE_URL=https://api.featherless.ai/v1
FEATHERLESS_MODEL=<chosen-model-id>
```

Never commit the real `.env` file or key.

### OpenAI-compatible example

```python
from openai import OpenAI
import os

client = OpenAI(
    base_url=os.environ["FEATHERLESS_BASE_URL"],
    api_key=os.environ["FEATHERLESS_API_KEY"],
)

response = client.chat.completions.create(
    model=os.environ["FEATHERLESS_MODEL"],
    messages=[{"role": "user", "content": "Hello"}],
)
```

This is only a connectivity pattern, not a product architecture decision.

### When to use Featherless

Use it only when AI directly improves the selected user problem, for example:

- explaining complex financial concepts in accessible Romanian;
- summarising or structuring user-provided financial information;
- generating personalised scenarios from structured inputs;
- conversational guidance where deterministic UI alone is insufficient.

Avoid adding an LLM merely because credits exist. The Stripe jury scores problem fit, UX, technical quality and pitch; an unnecessary model adds latency, uncertainty and failure modes.

## ChatGPT / Codex

Use for development assistance:

- architecture review;
- implementation tasks;
- debugging;
- tests;
- documentation;
- pitch/story refinement.

Keep tasks small and test generated code before merging.

## Secrets

Never place API keys in:

- frontend JavaScript bundles;
- GitHub commits;
- README screenshots;
- Discord messages;
- Lovable prompts if they are stored publicly;
- slide decks or demo recordings.

Use environment variables and provider secret stores.
