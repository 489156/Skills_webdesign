# Prompts

## Recreation prompt

Build a single-file, three-view HTML prototype for **UNDERSTUDY**, a product that captures an
outgoing business owner's operating knowledge during a 90-day ownership handover. No build step,
no external requests.

**Direction** — a working document, not a dashboard. Hairlines, square corners, no shadows except
on the one element meant to read as a phone. Color only what is risky.

- Tokens: paper `#edeeea`, panel `#f8f8f5`, ink `#1a2029`, muted `#576069`, accent teal `#0e6e6e`.
  Dark: paper `#101413`, panel `#171c1c`, ink `#e4e8e6`, accent `#37b3ae`.
  Semantic ramp kept separate from the accent: critical `#b4472e`, watch `#b5872a`
  (dark `#dd7a63` / `#d5a851`).
- Type: `ui-serif, Georgia` for display **and for every line the owner speaks**; system sans for
  UI prose; monospace for timecodes, labels, percentages, money. System stacks only.
- Theme: tokens on `:root`, redefined under `@media (prefers-color-scheme: dark)` and again under
  `:root[data-theme="dark"]` / `:root[data-theme="light"]` so a toggle wins in both directions.

**Masthead** — product mark, the deal (business, town, crew count, close date), `Day 34 of 90`,
and the seller-note end date. Then three tabs, each with a second line naming its state.

**View 1 · Prompt book** — 3 columns `236px / 1fr / 304px`.
Left: eight operating domains as an index, each with a coverage percentage, a 4px bar tinted by
risk, and an open-gap count; clicking one filters the gap list. Centre: `61%` continuity coverage
in the serif at ~86px, a sentence of definition, then a **spine** — eight segments whose *width is
revenue exposure* and whose *fill height is coverage*, tinted by risk. Below it, gaps ranked by
exposure: risk stripe, what is missing, where it lives now (`Verbal only — Bud Kessler`, the name
in the critical color), dollars exposed, and an `Add to agenda` toggle. Right rail: the next
22-minute session with an agenda you build from the gaps, an "if Bud stops answering tomorrow"
panel converting coverage into dollars / days / minutes owed, and a plain-language recording
notice.

**View 2 · Capture session** — transcript left, extracted facts right. The owner's turns are set
in the serif at 16px with key phrases marked; the agent's questions are muted sans. Each extracted
fact shows session, timecode, speaker, and two buttons — `Bud confirms` / `Needs correction` —
that change the card's state. Include a dashed **guardrail** note describing a moment the agent
stopped recording because the owner began discussing an employee's personal circumstances.

**View 3 · Crew view** — a phone-shaped card: a technician's spoken question, the answer in the
owner's own words with full provenance, and a `Hear Bud say it` control with a small waveform.
Beside it, a three-step explanation of how capture becomes the operating layer after day 90.

**Behavior** — tabs switch views; domain filter with a clear-filter affordance; agenda assembly
from gaps with a "slots remaining in 22 minutes" line; confirming a fact raises the coverage
number; counter respects `prefers-reduced-motion`.

**Responsive** — 1140px: rail drops below as two columns, session becomes stacked.
780px: single column, centre column first, per-row money hidden.

## Remix prompt

Same three-view structure, different domain: a **retiring cardiac sonographer at a rural hospital**
handing off to a replacement. Replace revenue exposure with clinical-risk exposure, the eight
operating domains with protocol/equipment/referral domains, and the crew view with a phone at the
bedside. Keep the guardrail visible and make the consent stricter, not looser.
