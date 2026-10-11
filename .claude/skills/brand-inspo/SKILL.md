---
name: brand-inspo
description: Interview the user thoroughly about their brand and messaging hierarchy, confirm a brief and search plan, then run the brand-identity-explorer agent to research three brand identity directions (industry-popular, bold, wild concept) with real brand, photography, architecture and art references.
---

# Brand identity inspiration

1. **Interview.** Read `.claude/design-research/intake.md` and run it in full: Rounds 1–3,
   Round 4b (identity) and Round 5. Ask in rounds, use `AskUserQuestion` for the closed choices, skip
   anything the user has already answered, and ask follow-ups on vague or conflicting answers.
   Don't start research until every must-have is answered or the user has said "you decide".

2. **Confirm.** Play back the brief, the search plan for each direction and the reference
   guidance. Wait for the user to confirm, and adjust if they ask.

3. **Hand off.** Save the confirmed brief to `inspiration/<project-slug>/brief.md`, then launch the
   `brand-identity-explorer` agent (Agent tool, `subagent_type: brand-identity-explorer`) with the file path, the full
   brief text and the user's links or images.

4. **Report back.** Pass on the agent's summary: the three direction titles with one-line ideas,
   the recommendation, and the report path. Offer to go deeper on one direction or to run
   `/logo-inspo` on the same brief.
