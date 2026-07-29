---
name: succession-deal-radar
description: Design the main screen of an opportunity-radar product — a scored, ranked feed of leads where each row carries the public evidence behind its score and the screen ends in one next action. Use for deal sourcing, off-market acquisition, prospecting, intent-signal, and lead-scoring dashboards where the list is the product.
---

# Succession Deal Radar

The main screen of a radar product has one job: turn "here is a market" into "call this person before lunch."
If the operator has to read the screen twice to know who to contact, the design failed.

## The screen model

Three zones, always in this order of importance:

1. **The read** — one modeled number, one sentence of consequence, one distribution chart. Above the list.
2. **The feed** — ranked rows. Score, evidence, money. This is the product.
3. **The next action** — a rail holding the selected item, why it scored, and a copy-ready first touch.

Filters live in a narrow left rail. They are a request slip, not a hero.

## Rules for the feed

- Rank by one primary score. Sort options change the order, never the columns.
- Every row shows **why**: 2 evidence chips pulled from source records, plus `+N` for the rest. Never show a score without its evidence.
- Mark the one signal that drives the score. Everything else stays muted.
- Money columns are right-aligned, tabular, and formatted at one scale (`$920K`, `$1.24M` — never `$1240K`).
- One row = one clickable target. Selecting a row updates the action rail, nothing else.
- Truncate names with ellipsis before you let a row grow taller. Row height is the density budget.

## Encode state in form, not just number

- A 3px severity stripe on the row's leading edge — read before any text.
- A conic-gradient dial for the score, colored by the same heat scale.
- Heat is a **semantic ramp** (cold / warm / hot) and is separate from the brand accent. Do not spend the accent on data.
- Put the heat scale legend in the filter rail. An unlabeled color ramp is decoration.

## Defaults that work

- Row padding `11px`, chip font `9.5–10px`, body `13–14px`, headline `clamp(21px, 2.4vw, 29px)`.
- Hairline rules (`1px`) between rows; solid border only around the selected row.
- Mono for every number, label, and ID. Sans for prose. One editorial serif line for the human quote.
- Transitions `160ms` on controls. One entrance animation (a counter, a bar rise), never both plus a fade.
- Breakpoints: 3-col → 2-col at `1120px` (action rail drops below) → 1-col at `760px` (feed first, filters second).

## The action rail

- Name the selected item, then answer "why this one" in one sentence, in plain language.
- Ship a **copy-ready script**, not a template with `{{merge_fields}}`. Operators send what they can read aloud.
- One primary button. Its label says what happens; after the click it says what happened.
- Below it: today's 3 moves with concrete times and counts, then a 4-stage funnel. Not a chart.

## Sourcing ethics — put it on the screen

A radar built on people needs its limits visible, not buried in a policy page. Footer, always:

- **Sources**: which public registries the score is built from.
- **Never**: personal addresses, home numbers, family records, scraped social profiles.
- **Opt-out**: the window, and that it applies platform-wide.

Label modeled numbers as modeled. Mask identities until the record is opened.

## Validate

- Can a new operator name the top target and their next action in under 10 seconds?
- Does every score have visible evidence, and does every evidence chip trace to a named source?
- Do filters produce an empty state that tells the operator which control to widen?
- Keyboard: rows reachable, focus visible, selection announced via `aria-current`.
- Both themes checked, reduced motion settles instantly, no horizontal body scroll at 420px.

## Avoid

- Cards with rounded corners and drop shadows. This is a ledger, not a feed.
- A giant hero that pushes row one below the fold.
- Repeating column labels inside every row on desktop.
- Scores with no evidence, or evidence with no source.
- Gauges, radars, and world maps that carry less information than a number would.
