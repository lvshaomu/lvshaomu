### Notes from running LLM workloads in production

I write down what breaks. Each repository below is a set of one-page recipes:
**Problem → Why it bites → Runnable code → Checklist**.

| Repository | What is inside |
|---|---|
| [llm-ops-recipes](https://github.com/lvshaomu/llm-ops-recipes) | Rate-limit pacing, a 15-second messaging window on 20–180s upstreams, the 180s timeout postmortem |
| [ai-agent-recipes](https://github.com/lvshaomu/ai-agent-recipes) | The agent loop, tool schemas that models call correctly, idempotent side effects, prompt injection defense |
| [dev-prompts](https://github.com/lvshaomu/dev-prompts) | 30 prompt cards for code review, debugging and test generation |

Everything is extracted from a live system: a multi-provider gateway serving 33 models across
free tiers, scheduled jobs that must survive unattended nights, and a messaging product with a
5-second reply window.

Free browser-only tools (nothing uploaded, works offline):
<https://csvtriage.com/box/>
