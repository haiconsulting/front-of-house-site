# Front of House — Design System

> The Open Door · October 2026 · Local review concept
> A restaurant studio with a welcoming, recognizable identity and a clear ownership promise.

This nine-section contract describes the marketing-site redesign authorized for
local review. It has **not** been approved for production or rollout across other
FOH applications. The user's current redesign brief supersedes the previous
visual direction. This file is the current brand reference where older design
checklists conflict.

Implementation sources: `src/styles/global.css` for tokens and
`src/components/Logo.astro` for the logo. Keep this contract aligned with both.
Use `.claude/craft/` for the universal quality bar. Commercial facts and pricing
remain in `src/data/site.ts`.

## 1. Visual Theme & Atmosphere

**The Open Door** is a geometric arch with an open door, paired with the stacked
lowercase wordmark **front of / house.** It signals welcome before a guest reaches
the restaurant. The identity should feel assured, useful, and rooted in hospitality.

Warm paper, deep red, substantial sans-serif type, generous spacing, and considered
photography carry the system. Use a distinctive composition rather than decorative
UI. Let the restaurant work demonstrate the studio's range.

## 2. Color

| Token | Value | Role |
|---|---|---|
| `--ember` | `#a52e24` | Signature red, logo, primary actions, selective emphasis |
| `--ember-deep` | `#84251f` | Red hover and active states |
| `--ink` | `#29251f` | Headings, structure, dark surfaces |
| `--paper` | `#f7f5ee` | Default warm background and reversed type |
| `--bone` | `#eeece3` | Secondary warm surface |
| `--body` | `#514c45` | Body text on light surfaces |
| `--muted` | `#756c62` | Secondary text on light surfaces |
| `--line` | `#d9d5ca` | Hairline borders |
| `--line-soft` | `#e7e3da` | Soft dividers |
| `--muted-on-ink` | `#d2c9bd` | Secondary text on dark surfaces |
| `--ink-border` | `#51483f` | Dark-surface borders |
| `--ember-bright` | `#efad99` | Legible accent on dark surfaces |

Supporting surfaces: `--toast: #e9e5da`, `--clay: #efe5dc`, and
`--dusk: #342a25`. Brass remains secondary and reserved for Care+ detailing:
`--brass: #8b672e`, `--brass-deep: #755520`. Status-only colors:
`--live: #75a17c` and `--danger: #a12424`.

Use semantic tokens. Spend red deliberately, with one clear primary action in a
view. Do not use dark red for small text on ink. Verify body contrast at 4.5:1,
large text and meaningful UI at 3:1, including interaction states.

## 3. Typography

- **Display and wordmark:** Archivo Variable. Strong, closely tracked headings;
  restrained weight in headlines, bold in the wordmark.
- **Body and UI:** Inter Variable. Clear, direct, and comfortable to scan.
- **Editorial accent only:** Cormorant italic, used sparingly for a short phrase.
  It is not the default heading or price face.

Live scale: H1 `clamp(3rem, 6.4vw, 6.6rem)`, H2
`clamp(2.2rem, 4vw, 4rem)`, H3 `clamp(1.35rem, 2vw, 1.8rem)`.
Headline leading is approximately `1.06`; display tracking is `-0.045em`.
Body text is at least 16px with `1.65` leading. Uppercase utility labels use
tracked Inter. Prices use tabular numerals. Do not force an italic accent into
every headline.

## 4. Spacing & Grid

- Content width: up to `1400px`, with `clamp(1.25rem, 4.4vw, 4rem)` gutters.
- Section padding: `clamp(4rem, 8vw, 7.5rem)`; tighter sections use
  `clamp(2.5rem, 5vw, 4.5rem)`.
- Default corner radius: `3px`. Prefer crisp, architectural edges to pill cards.
- Use whitespace and alignment before borders or shadows. Reflow deliberately
  for mobile, preserving text order and the primary action.

## 5. Layout & Composition

Lead with the guest's first impression and restaurant character. Bring real work
forward, then explain services, ownership, and transparent pricing. Avoid long
repeated feature blocks. One strong visual idea should organize each page.

Photography may be large and immersive. Real projects must use their real imagery
and accurate attribution. A generated fictional scene can establish the local
concept's mood when identified as such; it must never imply a client, testimonial,
or completed shoot. Generation provenance belongs in `public/brand/brand-notes.md`.

Keep readable menus, reservations, ordering, and discoverability tied to practical
guest needs. AI is a supporting capability, not the main identity.

## 6. Components

- **Logo:** geometric open doorway and stacked lowercase wordmark. Use the
  canonical SVG geometry from `Logo.astro`, keep proportions intact, and give it
  clear space. Red on paper, paper reversed, or a single-color version. Supply an
  accessible name on the containing link when the logo itself is decorative.
- **Buttons:** crisp `3px` corners, minimum `48px` height. Primary red with paper
  text; secondary transparent with a border; reversed paper on dark surfaces.
- **Cards:** quiet paper/bone surfaces, minimal borders, optional subtle shadow.
  Do not turn every paragraph into a card.
- **UI icons:** consistent SVG strokes and `currentColor`. The filled geometric
  brand mark is the intentional exception.
- **Forms:** persistent labels, actionable inline errors, clear pending and
  success states. Preserve working contact and lead-capture behavior.

## 7. Motion & Interaction

Keep motion short and purposeful, generally 150–250ms. Favor transform and opacity;
use subtle press feedback and clear hover states. All interactive elements need
visible keyboard focus. Respect reduced-motion preferences. Touch targets should
be at least 44px. Do not use animation to delay reading or access to an action.

## 8. Voice & Brand

Restaurant-native, warm, confident, and specific. Explain how the service helps
owners and guests. Avoid jargon, exaggerated outcomes, and invented evidence.

- Brand name: **Front of House**; **FOH** when a short form helps.
- Position: a web and brand studio built exclusively for restaurants.
- Core promise: a custom website the restaurant owns, with clear annual care.
- Current commercial facts: builds from **$2,000**, **Care $450/year**, and
  **Care+ $900/year**. Use `site.ts` as the pricing source.
- Assistant name: **the Host** in running copy, **The Host** in headings. AI drafts
  changes and the team reviews them before publication. Do not imply local models,
  instant publication, unlimited usage, or round-the-clock human support.
- Prefer a specific action such as “Start your project” or “Explore our work.”
- No em dashes in customer-facing copy. Use commas, colons, or periods.

## 9. Anti-patterns

- No invented reviews, customer counts, revenue lifts, rankings, or guarantees.
- No unsupported claims about competitors or universal performance claims.
- No fictional scene presented as a real client, room, team, or case study.
- No stock SaaS gradient, decorative emoji icons, excessive rounded tiles, or
  repeated ornamental flourishes.
- No claim that annual care means no recurring cost. State build and care together.
- No automatic cross-product rollout. Review this local concept first, then apply
  an approved identity consistently to the marketing site and relevant applications.
