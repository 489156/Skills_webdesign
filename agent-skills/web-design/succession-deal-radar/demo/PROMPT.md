# Prompts

## Recreation prompt

Build a single-file HTML main screen for **OFFMARKET**, a deal-radar product for acquisition
entrepreneurs hunting unlisted "boring" local businesses whose owners are near retirement.
No build step, no external requests, everything inline.

**Direction** — county records office meets a trading terminal. Hairline rules, no rounded cards,
no shadows.

- Palette tokens: ground `#e9eae4`, panel `#f6f6f2`, ink `#14181f`, muted `#5a6560`,
  accent ledger-green `#14624a`. Dark theme: ground `#0d100e`, panel `#141815`, ink `#e6eae3`,
  accent `#45c395`.
- A separate semantic heat ramp for succession urgency: cold `#3d6b8c`, warm `#b07c1e`, hot `#9e2b20`
  (dark: `#6fa0c4` / `#d6a344` / `#e0705f`). Never use the accent for data.
- Type: monospace as the display face (numbers, labels, headline), system sans for prose,
  `ui-serif, Georgia` italic for one owner-insight quote. System stacks only.
- Theme handling: define all color as custom properties on `:root`, redefine under
  `@media (prefers-color-scheme: dark)`, then again under `:root[data-theme="dark"]` and
  `:root[data-theme="light"]` so a toggle overrides the OS in both directions.

**Layout** — status bar, then a 3-column grid `206px / 1fr / 292px`.

- Left "search filter" rail: trade chips, a succession-score slider, a max-asking-multiple slider,
  and a heat-scale legend.
- Center: a modeled headline that counts up to `1,284`, a supporting paragraph, a 6-bar
  "modeled sell window, next 18 months" distribution, sort controls, a column header row, and a
  ranked feed of 9 businesses.
- Each row: 3px heat stripe, masked business name (`H——— Heating & Cooling`),
  a facts line (city · trade · est. year · asking multiple), two evidence chips from public records
  plus `+N`, then tenure / revenue / owner earnings columns, a conic-gradient score dial, and
  an "Open file" affordance. Right-align money, tabular numerals, `$920K` and `$1.24M` scaling.
- Right rail: the selected business, a serif italic sentence explaining why it scored, a
  copy-ready outreach script in a mono block, one primary button, then "Today · 3 moves"
  and a 4-stage funnel.
- Footer: sources used, data never used, and the opt-out window.

**Behavior** — chips and sliders filter live; sort by score / earnings / tenure; selecting a row
updates the right rail; the primary button flips to a confirmed state; counter respects
`prefers-reduced-motion`. Empty state names the control to widen.

**Responsive** — at 1120px the right rail drops below as two columns and tenure/action columns hide;
at 760px single column with the feed first, filters second, and per-row column labels appear.

## Remix prompt

Same screen, different market: retarget the radar at **independent pharmacies facing PBM
contract renewals**. Keep the layout, heat ramp, and evidence-chip pattern. Replace the trades with
pharmacy segments, the succession score with a "contract distress score", and the record signals
with public ones (state board licence status, DEA registration age, Medicaid provider enrollment,
lease term). Rewrite the outreach script for a buyer who keeps the pharmacist on staff.
