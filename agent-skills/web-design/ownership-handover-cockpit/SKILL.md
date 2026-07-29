---
name: ownership-handover-cockpit
description: Design screens for knowledge-transfer and continuity products — where the deliverable is what one person knows, coverage is the primary metric, and every fact must carry consent and provenance. Use for handover, onboarding-a-successor, tribal-knowledge capture, interview-capture, and any interface where an expert's own words are the asset.
---

# Ownership Handover Cockpit

The product is someone's memory, moved. That changes three things about the design:
coverage replaces progress, provenance replaces polish, and the person being recorded is a
**user**, not a data source.

## The three screens this pattern needs

Ship all three or the product reads as a note-taking app.

1. **The book** — what is captured, what is still in one head, and what the gap costs.
2. **The capture session** — the expert's own words, and their explicit act of confirming.
3. **The point of use** — the same knowledge one day later, where the work happens.

Screen 3 is what makes the product recurring. Skip it and you have shipped a document.

## Coverage is the metric — weight it by consequence

- Weight coverage by **revenue or risk exposure, not page count**. 400 documented pages of
  compliance boilerplate is not more coverage than one pricing rule worth $412K.
- Break it into named domains the operator already recognizes (customers & pricing, site quirks,
  vendors, collections, seasonality). Eight is about right; twelve is a taxonomy nobody reads.
- Show composition, not a donut: a segmented spine where each segment's **width is exposure**
  and its **fill is captured**. Low fill on a wide segment is the whole story.
- Convert coverage into consequence somewhere on the screen — dollars, days remaining, minutes of
  the expert's time still owed. A percentage alone tells an operator nothing about whether to panic.

## Rank gaps, not tasks

Each gap row carries: what is missing, **where it currently lives** (`Verbal only — Bud Kessler`),
what it exposes, and one action. Sort by exposure. The interface's job is to convert an anxiety
into a 22-minute agenda, so make the agenda assemblable from the list itself.

## Treat the outgoing expert as the author

This is the design decision that decides whether the product works.

- **Their words get the best typography on the page.** Set captured speech in the serif at the
  largest size in the view; set the system's questions in the muted sans. The transcript is
  testimony, not log output.
- Confirmation is **their act, attributed to them** — `Bud confirms`, never "verified".
- Nothing enters the book unconfirmed, and every fact shows session, timecode, and speaker.
- Open with what they are proud of, not with the highest-risk gap. Cap sessions at ~22 minutes.
- Before asking for anything, show them what they get: who keeps their job, what keeps its name.
- Never require them to type.

## Consent and guardrails belong on screen

Not in a policy page. In the interface, where the buyer and the expert can both see them:

- Signed consent, with the revocation window stated in days.
- An explicit **out-of-scope list** — employee performance, health, family, personal finances.
- **Render the guardrail firing.** When capture declines to record something, show that it
  declined and why. A visible refusal is the strongest trust signal an interface can produce.
- Say who owns the resulting knowledge, and that it transfers with the business.

## Visual defaults

- Color only what is risky. If everything is colored, nothing is. Calm is the absence of color.
- One semantic ramp (`critical` / `watch`) kept strictly separate from the brand accent.
- Serif display + serif for captured speech, system sans for UI prose, mono for timecodes,
  IDs, percentages, and money. The mix is the point: three voices, three faces.
- Hairlines, square corners, no shadows except on the one thing meant to read as a device.
- Tabs carry a second line naming the view's state (`Session 11 · in progress`) — in a
  time-boxed product, where you are in the clock is primary information.
- Breakpoints: 3-col → 2-col at 1140px → 1-col at 780px with the centre column first.

## Validate

- Can the operator state, in one sentence, what breaks if the expert disappears tomorrow?
- Does every fact on screen trace to a speaker and a timecode?
- Is there a screen the expert would be willing to read before agreeing?
- Does a guardrail event appear anywhere in the interface?
- Keyboard reachable, `aria-selected` on tabs, both themes, reduced motion settles instantly.

## Avoid

- Progress bars for knowledge. Progress implies a known denominator; coverage is an estimate.
- Anonymous facts. "The system found" is worthless; "Bud said, session 11, 11:59" is an asset.
- Treating the expert as content. They can walk away, and then the product has nothing.
- A capture screen with no point-of-use screen. That is a document, sold as software.
