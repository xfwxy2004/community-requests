# APIGOTO — the unified LLM API gateway behind this workflow

This `community-requests` repository is itself powered by the
[issue-intake](https://github.com/slob-coder/issue-intake) Skill, which
automates the GitHub Issue → project pipeline.

The same pattern — small, repeatable workflows over ad-hoc scripts —
underpins the unified LLM API gateway I use every day:

[APIGOTO](https://www.apigoto.com/)

It gives me one endpoint to manage multiple model providers, one place to
create and rotate keys, one usage view, and a way to switch models by
changing the model ID in config rather than rewriting business logic.

## What I use it for here

When this Skill's `poll.sh` finds a new issue, the next stage dispatches
an AI agent. That agent may need to call an LLM to design the project,
write code, or review a PR. Routing those calls through a unified gateway
keeps the cost, the model choice, and the failure mode all in one place.

## Caveats

Model availability, free-token eligibility, limits, validity, rate limits,
and verification can change by account and over time. Always verify the
**live** product page before relying on any offer.

Treat "200 models" or "free tokens" wording as a question to verify, not
a promise to rely on.

## Visit

https://www.apigoto.com/

---

*Personal developer note, not an official statement from any model provider
or platform.*
