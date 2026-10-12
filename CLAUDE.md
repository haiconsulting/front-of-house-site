# Front of House — Website

Astro marketing site for Front of House, the restaurant web studio.

**Current direction: The Open Door, October 2026.** The user authorized a full
brand and marketing-site redesign for local review at port 4999. This concept is
pending user approval before production or rollout across other FOH applications.
The current `FOH-DESIGN.md`, `src/styles/global.css`, and
`src/components/Logo.astro` supersede legacy palette, type, and logo requirements
in older checklists. Preserve the craft requirements that do not conflict.

## Design contract — read before any visual or copy work

**Start with `Mac_Master_Design_claude_must_read.md`** (project root): the
master doc that unifies all design guidance, sets the order of authority,
and carries the merged pre-delivery checklist. It layers two installed
skills on top of the contract below: `.claude/skills/frontend-design/`
(design process, anti-default thinking) and `.claude/skills/ui-ux-pro-max/`
(searchable UX/color/type database + Astro stack rules; its style generator
never overrides a brand contract).

Any agent generating or editing UI, layout, styling, imagery, or copy for this
project MUST work against two sources of truth:

1. **`FOH-DESIGN.md`** (project root) — the FOH brand contract in the Open Design
   9-section schema: color tokens, typography, spacing, components, motion, voice,
   and anti-patterns. This defines *what FOH looks and sounds like*.
2. **`.claude/craft/`** — universal, brand-agnostic craft rulebooks that apply on
   top of the brand contract. These define *the quality bar a competent designer
   holds regardless of brand*.

The live design tokens are in `src/styles/global.css`. `FOH-DESIGN.md` mirrors
them — if you change one, change the other.

### Which craft file to consult when

| Working on… | Read |
|---|---|
| Any marketing/landing surface | `.claude/craft/anti-ai-slop.md` |
| Any typed content | `.claude/craft/typography.md` + `typography-hierarchy.md` |
| Long-form reading (blog, about, docs) | also `typography-hierarchy-editorial.md` |
| Any styled output | `.claude/craft/color.md` |
| Motion, transitions, micro-interactions | `.claude/craft/animation-discipline.md` |
| Pricing, dashboards, onboarding, modals | `.claude/craft/laws-of-ux.md` |
| Any interactive UI (focus, labels, keyboard) | `.claude/craft/accessibility-baseline.md` |
| Any form (contact, lead capture, intake) | `.claude/craft/form-validation.md` |
| Stateful UI (lists, tables, loading, empty) | `.claude/craft/state-coverage.md` |

### Non-negotiables (fast checklist)

- Use The Open Door mark from `src/components/Logo.astro`: geometric arch and
  open doorway, stacked lowercase `front of / house.` wordmark.
- Signature red `#a52e24`, ink `#29251f`, paper `#f7f5ee`, bone `#eeece3`.
  Read complete semantic tokens from `src/styles/global.css`.
- Archivo Variable for display and wordmark; Inter Variable for body/UI.
  Cormorant italic is an occasional editorial accent only.
- Compose around hospitality, real work, and ownership. Keep services and pricing
  clear: a one-time build from $2,000, then annual Care from $450.
- Use crisp edges, deliberate spacing, restrained motion, visible focus, readable
  contrast, and mobile touch targets. Verify the page in a browser at mobile and
  desktop widths, including reduced motion and keyboard navigation.
- Use SVG UI icons, not emoji. Preserve the logo's intentional filled geometry.
- Use real project imagery for case studies. Identify any fictional generated
  concept photography and document its provenance in `public/brand/brand-notes.md`.
- No invented metrics, endorsements, search guarantees, or claims about competitors.
- The AI assistant is **the Host**. AI drafts changes; the team reviews them.
- No em dashes in customer-facing copy. Avoid generic repeated feature-card layouts.
- Keep this phase local and reviewable. User approval is still pending for the
  production identity and its application to other FOH products.

> This design contract was seeded from the Open Design toolkit
> (`Claude Design/open-design`, `craft/` + 9-section `DESIGN.md` schema).
> To refresh the craft rulebooks, re-copy from that repo's `craft/` folder.


## FOH work log (required)

When you finish meaningful work, append one line so Chamber 2 can brief Drew:

```bash
~/.redmax/chambers/bin/worklog "what you did"
```

That writes this project's `WORKLOG.md` and `~/Desktop/FrontOfHouse/.foh-worklogs/index.jsonl`.
Append only. Do not rewrite history.
