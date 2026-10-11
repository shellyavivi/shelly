# Design inspiration

Reports from the design research agents land here, one folder per project.

| Command | Agent | Output |
|---|---|---|
| `/logo-inspo` | `.claude/agents/logo-explorer.md` | `inspiration/<project>/<date>-logo.md` |
| `/brand-inspo` | `.claude/agents/brand-identity-explorer.md` | `inspiration/<project>/<date>-brand-identity.md` |

Each command first interviews you in a few short rounds: business, message, audience,
competitors, visual limits, how far to push, and logo or identity specifics. It then plays back
the brief and a search plan for you to confirm. The brief is saved as `inspiration/<project>/brief.md`.

Each report turns your messaging hierarchy (core idea → pillars → tone → audience → constraints)
into three directions:

1. **Proven** — the category done at its best
2. **Stand Out** — breaks one category convention on purpose
3. **Concept** — starts from a metaphor or idea instead of the category

Each direction includes real brands, photography, architecture and art. Every link is checked, the
key images are looked at, and each set is checked so the references work together.
The shared method is in `.claude/design-research/playbook.md`; edit it to change sources or format.
