---
name: logo-inspo
description: Collect a messaging hierarchy from the user, then run the logo-explorer agent to research three logo directions (industry-popular, bold, wild concept) with real brand, photography, architecture and art references.
---

# Logo inspiration

1. **Get the messaging hierarchy.** If the user already gave it (in the args or the conversation),
   use it. Otherwise ask for it in one message, in this order, and say that short answers are fine:
   - Project / brand name, and what it does
   - **Core idea** — the one thing the brand must say
   - **Pillars** — 2–4 supporting messages or values, most important first
   - **Personality / tone** — 3–5 adjectives
   - **Audience**
   - **Constraints** — must / must-not, competitors, existing assets, where the logo must work
   Don't hold things up for missing levels; the agent will infer and label them `(assumed)`.

2. **Delegate.** Launch the `logo-explorer` agent (Agent tool, `subagent_type: logo-explorer`) with
   the full hierarchy word for word, plus any reference images or links the user shared.

3. **Report back.** Relay the agent's summary: the three direction titles, one-line ideas, the
   recommendation, and the report path under `inspiration/`. Offer to go deeper on one direction
   or to run `/brand-inspo` on the same brief.
