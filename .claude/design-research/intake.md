# Design Research Intake

Used by `/logo-inspo` and `/brand-inspo` **before** any research starts. The research agents can't
ask questions mid-run, so everything that changes *what to search for* must be settled here.

Goal: understand the brief well enough to write a search plan you'd stand behind. Don't stop
after the minimum. Keep asking until every **must-have** below is answered or the user has
said "you decide" for it.

## How to run it

- **Ask in rounds, not as one wall of questions.** Use 3–4 rounds with 4–7 questions each,
  numbered so the user can answer quickly.
- **Use `AskUserQuestion` for closed choices** (stage, risk appetite, archetype, how wild to go).
  Use plain numbered questions for open answers.
- **Skip what's already known.** Read anything the user already shared (brief, deck, links, images,
  earlier messages) and only ask what's still open. Say what you already took from it.
- **Push on vague words.** Answers like "modern", "clean", "premium", "minimal", "bold",
  "friendly" don't say what to search for. Ask what they mean with a contrast
  ("premium like Aesop, or premium like Rolex?") or by asking for a brand that shows it.
- **Push on conflicts.** If two answers pull against each other (e.g. "playful" and "authoritative",
  or "stand out" while naming only category-standard brands they like), point it out and ask
  which one wins.
- **Accept "you decide."** Record it as `(open, agent decides)` rather than asking again.

## Round 1 — The business and the message (must-have)

1. Brand name. What it does, in one sentence. What industry or category it's in.
2. Stage: new brand, refresh, or full rebrand? If it's a rebrand, what's wrong with the current one?
3. **Core idea:** the one thing people should feel or believe about the brand.
4. **Pillars:** 2–4 supporting messages, ranked. What proves each one is true?
5. **Personality:** 3–5 words for what it is, and 3 words for what it must never feel like.
6. Why now? What changed that made this project happen?

## Round 2 — People and market (must-have)

1. Main audience: who they are, age range, and what they care about. Any secondary audiences?
2. Which other brands, apps, shops or media does this audience already love?
3. Where it will be used: countries and languages. Any script needs (Hebrew, Arabic, CJK…)?
   Any cultural meanings to avoid?
4. 3–5 direct competitors. How should this brand look different from them?
5. Brands they admire, **inside and outside the category**, and what exactly they admire about each.
6. Brands or styles they dislike, and why.

## Round 3 — Visual boundaries and ambition (must-have)

1. Existing assets that must stay or can change: name, logo, colours, fonts, photography.
2. Colours they want, colours that are banned, and colours competitors already own.
3. Risk appetite for the final choice (`AskUserQuestion`): play safe / distinctive but safe /
   push hard.
4. How wild should the **Concept** direction go (`AskUserQuestion`): grounded twist /
   unexpected but buildable / fully experimental.
5. Photography, architecture, art, film or places they love, or ones to avoid.
   This steers the non-design references.
6. Any references they've already collected (links, images, Pinterest or Are.na boards)?

## Round 4a — Logo specifics (`/logo-inspo`)

1. Type of mark (`AskUserQuestion`, multi-select): wordmark / monogram / symbol / combination /
   emblem / open.
2. Does the name have a meaning, origin or story the mark could use?
3. Hardest places it must work: favicon/app icon, embroidery, engraving, signage, packaging,
   animation, social avatar.
4. Must it pair with an existing typeface or brand system?
5. Will it carry sub-brands or a family of products?

## Round 4b — Identity specifics (`/brand-inspo`)

1. Main touchpoints, ranked: digital product, website, packaging, retail or physical space,
   social, OOH, events, merch, print.
2. Imagery: will they shoot their own photos, use stock, illustration, 3D or product renders?
   Is there a budget for art direction?
3. Is motion or sound important (app, video, social)?
4. Production limits: print finishes, materials, sustainability rules, in-house team skills.
5. Tone of voice: are there copy examples they love, or brand voices to avoid?
6. Is there a logo already? If not, should the identity directions include logo thoughts?

## Round 5 — Practical (ask briefly, in any round)

- Deadline and what the report is for (internal kick-off, client presentation, personal project).
- Anything that would make them reject a direction straight away?

## Play back and confirm (always)

Before handing off to an agent, show the user:

1. **The brief** as the hierarchy table (core idea → pillars → personality and anti-personality →
   audience → constraints), with each `(open, agent decides)` item marked.
2. **Search plan:** for each of the three directions, the angle you'll take and 4–6 search themes
   or keywords. For the Concept direction, include 2–3 candidate metaphor territories.
3. **Reference guidance:** which kinds of photography, architecture and art to look for, and
   what to avoid.

Ask: "Anything to change before I start the research?" Adjust and confirm again if needed.

## Hand-off

Save the confirmed brief and search plan to `inspiration/<project-slug>/brief.md`. Pass the
agent both the file path and the full brief text, plus any links or images the user shared.
