# Design Direction Research — Shared Playbook

Both `logo-explorer` and `brand-identity-explorer` follow this playbook. Read it fully before starting.

---

## 1. Decode the messaging hierarchy

The brief comes from the intake interview (`.claude/design-research/intake.md`), usually saved at
`inspiration/<project-slug>/brief.md` with a confirmed search plan. Read it in full, and treat the
search plan, the admired/disliked brands and the reference guidance as binding. Normalise the
brief into this table before searching:

| Level | Meaning | Example |
|---|---|---|
| **1. Core idea / promise** | The one thing the brand must say | "Energy you can see" |
| **2. Supporting pillars** | 2–4 proof points or values | Transparency · Calm control · Home-first |
| **3. Personality / tone** | How it sounds and feels | Warm, precise, quietly confident |
| **4. Audience** | Who it speaks to | Design-literate homeowners, 30–50 |
| **5. Constraints** | Must / must-not, category, competitors, existing assets | No green leaves, must work at 16px |

Then turn the hierarchy into a **visual vocabulary**: for each level, list 3–5 visual translations
(form, material, light, rhythm, colour temperature, typographic voice). The core idea drives the
primary form; pillars drive secondary devices; tone drives typography and colour; constraints filter.

Items marked `(open, agent decides)` are yours to decide; state your choice and why. If something
is still missing (e.g. the agent was launched without the intake), infer it, mark it `(assumed)`,
and list it under **Open questions** at the end of the report so the user can correct course.
You can't ask the user mid-run, so keep going.

## 2. The three directions

Every report has exactly three directions, each answering the same hierarchy:

1. **Industry Popular — "Proven"**
   What the strongest players in and around the category do right now. Executed at the top of the
   craft, not the average. Goal: credible, low-risk, instantly legible. Say which category
   conventions it follows and why that is useful here.

2. **Bold — "Stand Out"**
   Takes one convention of the category and breaks it on purpose (colour, scale, typography,
   motion, tone). Still clearly commercial and shippable. Name the convention being broken.

3. **Go Wild — "Concept"**
   Starts from a conceptual idea, not from the category. Find a metaphor, system, material,
   phenomenon or cultural reference that embodies the core idea and build the direction from it.
   Give the concept a name and a one-sentence rationale. It can be impractical; it must be
   intellectually coherent and traceable back to level 1 of the hierarchy.

Directions must be genuinely different from each other — if two would share a moodboard, push
the bold one further and the wild one into a different domain.

## 3. Where to search

Use `WebSearch` + `WebFetch`. Search in several sources per direction; do not lean on one site.

**Design platforms (primary)**
- Brand New / UnderConsideration (underconsideration.com/brandnew) — reviewed identity launches
- BP&O (bpando.org) — critical identity reviews
- It's Nice That (itsnicethat.com), Creative Boom, Design Week, Creative Review
- The Brand Identity (the-brandidentity.com), Identity Designed (identitydesigned.com)
- Fonts In Use (fontsinuse.com) — real type pairings in the wild
- Behance curated galleries (behance.net/galleries), Dribbble (logos only, sparingly)
- Logo Lounge trend reports (logolounge.com), Logobook (logobook.com) — logos
- D&AD, Type Directors Club, Brand Impact Awards, ADC — award-winning work
- Savee, Cosmos, Are.na, Mindsparkle Mag, Siteinspire — mood and art direction

**Studios worth scanning** for top-tier precedents: Pentagram, Collins, Wolff Olins, Koto, DesignStudio,
Order, Mucho, Base Design, Sagmeister & Walsh, Studio Dumbar, Snøhetta, Lundqvist, Porto Rocha,
Ragged Edge, Mother Design, Interbrand, Landor, Jones Knowles Ritchie, Manual, Hey Studio.

**Required image sources — every direction must include at least:**
- **2 Behance projects** (behance.net/gallery/...), preferably from curated galleries or featured work.
- **2 big-studio case studies** (Pentagram, Collins, Koto, Porto Rocha, Wolff Olins, DesignStudio,
  Mucho, Base Design, Order, Studio Dumbar, Snøhetta, Landor, JKR…), linking to the studio's own page.
- **2–3 Pinterest pins**: individual pin URLs (pinterest.com/pin/...), found with `WebSearch`
  (e.g. `site:pinterest.com/pin <query>`). Pinterest pages often block fetching. In that case, cite a
  pin only if the search result clearly shows what it is, and say it couldn't be fetched. Where you
  can, trace the pin back to its original source and cite that as well.

**Outside design (required for every direction)**
- **Photography** — named photographers and series (e.g. Wolfgang Tillmans, Hiroshi Sugimoto, Saul
  Leiter, Rinko Kawauchi, Andreas Gursky, Bernd & Hilla Becher, Vivian Maier).
- **Architecture** — named buildings and architects (e.g. Tadao Ando's Church of the Light, SANAA's
  Rolex Learning Center, Zaha Hadid, Lina Bo Bardi's SESC Pompéia, Peter Zumthor's Therme Vals).
- **Art** — named works and artists (e.g. Josef Albers' *Homage to the Square*, James Turrell,
  Olafur Eliasson's *The Weather Project*, Sol LeWitt, Ellsworth Kelly, Agnes Martin, Yayoi Kusama).
- Optional: product/industrial design, fashion, film stills, nature/science imagery.

Museum and institution pages (MoMA, Tate, Guggenheim, Getty, ArchDaily, Dezeen, Magnum, Aperture)
are preferred sources for non-design references.

## 4. Reference rules — real, good, cohesive

**Real.** Every reference must be an existing brand, work, building, or photograph with a working URL.
- No invented brands, no AI-generated imagery, no "imagine a logo that…" as a reference.
- `WebFetch` each URL you cite. If it 404s or is paywalled with no visible content, replace it.
- Prefer the original source (studio case study, museum page) over aggregators/Pinterest.

**Good.** Quality bar = work you'd show a creative director.
- Prefer award-winning, reviewed, or studio-published work. Avoid template marketplaces, spec work
  with no client, and low-effort Dribbble shots.
- Visually check the key references: grab the page's `og:image` (or main image) URL from the fetched
  page, download it into the session scratchpad (or `/tmp/design-refs/`) with `curl -sL -o`, then
  open it with `Read` to actually look at it. Drop anything that looks dated, messy or off-tone.
  Do this for at least the hero reference + 2 others per direction.

**Cohesive.** Each direction is a curated set, not a pile.
- After collecting, run a **cohesion check** per direction: shared colour temperature? compatible
  form language? one typographic voice? consistent light/texture? If one reference fights the
  others, cut or replace it.
- Write a 1-line "why these belong together" for each direction.
- Across directions, references should *not* overlap.

**Visual.** The report must show images, not only links. Embed each reference's image as
`![short caption](direct image URL)` using the page's `og:image` or the CDN URL
(`mir-s3-cdn-cf.behance.net`, `i.pinimg.com`, the studio's own image host), followed by the source link.
Only embed images you've viewed and approved.

## 5. Output

Save the report as Markdown to:
`inspiration/<project-slug>/<YYYY-MM-DD>-<logo|brand-identity>.md`
(create folders as needed). Then return a short summary plus the file path to the caller.

Report skeleton:

```markdown
# <Project> — <Logo | Brand Identity> Exploration
_Date · Agent_

## Brief, decoded
<hierarchy table> + visual vocabulary bullets

## Direction 1 — Proven: <title>
**Idea:** one sentence. **Category conventions used:** …
**Why it answers the brief:** maps to hierarchy levels 1–3.

### Hero reference
### Brand references (3–5)       — name · studio/agency · year · link · what to take from it
### Behance (2+) · Studio case studies (2+) · Pinterest (2–3) — embedded image · source · what to take
### Photography (1–2)            — photographer · series/work · link · what to take
### Architecture (1–2)           — building · architect · link · what to take
### Art (1–2)                    — artist · work · link · what to take
### Palette / type / form cues   — concrete: hex ranges, type families or classifications, shapes
### Cohesion note                — why these belong together
### Risks                        — where it could go generic or wrong

## Direction 2 — Stand Out: <title>
… same structure, plus **Convention broken:** …

## Direction 3 — Concept: "<concept name>"
… same structure, plus **Concept:** the metaphor and how it traces to the core idea

## Side-by-side
| | Proven | Stand Out | Concept |
|---|---|---|---|
| Risk | | | |
| Memorability | | | |
| Fit to core idea | | | |
| Best for | | | |

## Recommended next step
Which direction(s) to sketch first and what to test.

## Open questions
Assumptions you made, and questions whose answers would change the research.

## Sources
Every URL used, grouped by direction.
```

"What to take from it" must be specific (e.g. "the way the counter of the 'a' becomes the
symbol", "the warm 3200K side-light on raw concrete"), never "nice vibe" or "clean look".
