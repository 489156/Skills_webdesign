# UNDERSTUDY — Concept, Commercialization Review, and Business Case

**Status:** prototype complete; direction changed at M2; two claims withdrawn at M5
**Date:** 29 July 2026
**Predecessor:** OFFMARKET Deal Radar (killed at M2 — see §5)

> **Revision note, 30 July 2026.** Market research after this document was first written
> ([MARKET-RESEARCH.md](MARKET-RESEARCH.md)) invalidated the lender-channel thesis and showed the
> capture mechanic is already commoditized in consumer products. Affected passages are marked
> ⚠ **WITHDRAWN** below rather than deleted, so the reasoning error stays visible. Strategy
> revisions are in [MEETING-MINUTES.md](MEETING-MINUTES.md).
>
> All financial figures in this document are **modeled assumptions**, labeled as such.
> Nothing here is measured revenue. The market-size and transition-volume figures are
> sourced in [REFERENCES.md](REFERENCES.md); everything derived from them is our model.

---

## 1. The one-sentence identity

**UNDERSTUDY captures the outgoing owner's head before it walks out the door, and turns it
into how the business answers itself afterwards.**

Not a marketplace. Not a CRM. Not a deal-sourcing tool. The product is **operating continuity
across a change of ownership** — sold as a fixed-scope 90-day engagement, retained as a
subscription.

What it is not, stated on purpose:
- Not a data broker. We never score, rank, or profile a natural person.
- Not a field-service management system. We sit next to Jobber/ServiceTitan, not against them.
- Not consulting. Humans do QA, agents do capture. If we ever staff-bill, the model is broken.

---

## 2. The team (personas with kill authority)

Each persona holds a veto on their domain. "Kills" are the things they will not let ship.

| Persona | Role | Formative experience | Bias to correct for | Will kill |
|---|---|---|---|---|
| **Ye-jin Park**, 31 | Founder / CEO | Bought and exited a $2.4M commercial laundry route as a self-funded searcher | Over-indexes on their own search experience | Anything with a 24-month sales cycle |
| **Marcus Oyelaran**, 38 | Head of Data & Records | Built permit + licence ingestion across 140 US counties for a GIS contractor | Believes any public record can be normalized | Features needing per-county manual QA |
| **Sunhee Cho**, 43 | Head of Trust, Privacy & Compliance | Compliance lead at a consumer credit bureau (FCRA regime) | Assumes the worst-case regulator | **Any product that scores a natural person** |
| **Diego Ramirez-Hale**, 45 | VP Field Operations | 19 years running HVAC/plumbing branches; lived through 6 owner transitions | Distrusts anything crews must adopt | Any flow that requires a technician to type |
| **Aisha Bello**, 34 | Head of Growth | Built an acquisition-entrepreneurship channel to 180k subscribers | Believes content solves distribution alone | Paid-acquisition line items |
| **Jonas Weill**, 52 | Head of Capital Partnerships | Ex-SBA 7(a) credit officer, top-10 lender | Thinks every channel is a lender channel | Consumer-priced products |
| **Rin Takeda**, 29 | Design Lead | Information-dense operational tools | Density over onboarding | Dashboards with no next action |

**Added at M3** (the pivot created three gaps in the cast):

| Persona | Role | Formative experience | Will kill |
|---|---|---|---|
| **Halina Novak**, 47 | Voice & Knowledge Extraction Lead | Clinical speech capture with elderly patients | Any capture session over 22 minutes |
| **Tobias Reinhardt**, 41 | CFO / Unit Economics | Services-PE operator, rolled up 3 trade platforms | Engagements under 65% gross margin |
| **Priya Anand**, 36 | Counsel (M&A + employment) | Advised 40+ lower-middle-market deals | Capture that touches employee performance data |

### Customer & corporate personas

| Persona | Who | What they actually want | What makes them say no |
|---|---|---|---|
| **Cal Whitmore**, 33 | Self-funded searcher, Greenville SC. Closed a $3.1M septic company, SBA 7(a), 11 employees, 90-day seller-note transition. **The ICP.** | To not lose the accounts in month 7 | Another monthly subscription he has to justify to himself |
| **Bud Kessler**, 66 | The outgoing owner. 31 years, HVAC, Grove City OH. Will not type. Suspicious of "systems." | The crew keeps their jobs and the name stays on the trucks | Feeling replaced, or interrogated, or recorded without control |
| **Denise Okafor**, 49 | SVP Credit, regional SBA lender, $480M 7(a) book | Fewer charge-offs in months 6–18 post-close | Anything that slows a closing or adds a covenant they must police |
| **Ramona Fitzgerald**, 58 | Director, county Small Business Development Center (B2G) | Measurable jobs retained per dollar of program funds | A vendor who can't produce a per-business outcome report |

---

## 3. Milestone log

| # | Milestone | Gate criteria | Outcome |
|---|---|---|---|
| M0 | Charter & cast | Personas hold explicit veto | Done |
| M1 | Identity & ICP lock | One identity sentence, one named ICP, a demand mechanism that isn't market size | **Failed twice, then passed** |
| M2 | Stricter feasibility gate | Survive unit economics + legal + retention | **FAILED — direction changed** |
| M3 | Prototype implementation | Screens a real buyer can operate | Done — 3 views, shipped |
| M4 | Documentation + proposal | Submittable to a named customer | This document + [proposal](proposal/index.html) |
| M5 | **Market research + strategy** | Prove the square is empty; find prior art | **Two claims invalidated** — [MARKET-RESEARCH.md](MARKET-RESEARCH.md), [MEETING-MINUTES.md](MEETING-MINUTES.md) |

---

## 4. Meeting 1 — Identity and ICP (end of M1)

**Subject on the table:** OFFMARKET Deal Radar — off-market deal sourcing for acquisition
entrepreneurs.

**Ye-jin Park:** "I was this customer. I would have paid for this. But I paid for it *for
nine months* and then I stopped forever, because I bought the thing. Our best possible outcome
is that our customer succeeds and leaves."

**Aisha Bello:** "The content engine is real — this audience is enormous and starving. But I'd
be filling a bucket with a hole in it."

**Jonas Weill:** "Nobody in credit will touch a product priced at $250 a month. That's an
expense-report product, not a partnership. And I can't refer buyers to a tool that helps them
find deals — my institution's interest is in the loan performing after the close, not before."

**Marcus Oyelaran:** "The data is achievable, but per-metro. Every county formats records
differently. Fifty metros is fifty integration projects, not one product."

**Sunhee Cho:** *(the veto)* "Stop. Read our own screen. We're computing a 'succession score'
for a named individual, from licence renewals and officer filings, and selling it to people who
want to transact with them. That's a profile of a natural person, built without their knowledge,
sold to third parties, used to make a decision about them. Whether or not it's technically a
consumer report today, I will not sign it. And 'public records only' is not a defense — it's
where every data-broker enforcement action starts."

**Rin Takeda:** "Design-wise the screen works. It answers 'who do I call.' The pattern is
worth keeping regardless of what happens to this business."

**Decision:** M1 passed on ICP clarity (Cal Whitmore is a real, findable, specific customer)
but flagged three structural problems for the M2 gate:
1. Success-equals-churn retention
2. Negative in-market network effects — every additional customer in a metro competes with the
   others for the same owners, so the product gets worse as it sells
3. An unresolved compliance veto on the core scoring object

**Incorporated:** the M2 gate criteria were tightened before the meeting closed — a hard
requirement was added that the scored object must be a *business event*, never a person.

---

## 5. Meeting 2 — The stricter gate, and the kill (end of M2)

### 5a. OFFMARKET, scored against the gate

| Criterion | Threshold | OFFMARKET | Verdict |
|---|---|---|---|
| Net revenue retention | ≥ 100% | ~35–50% modeled (churn on success) | **Fail** |
| Serviceable revenue at realistic share | ≥ $150M | ~$90M ceiling at 100% share; <$10M realistic | **Fail** |
| Marginal cost to add a market | Near zero | One integration project per metro | Fail |
| Network effect | Positive | **Negative within a market** | **Fail** |
| Legal object | Not a natural person | A named owner's likelihood of exiting | **Fail (veto)** |
| Channel with aligned incentive | Exists | Lenders decline; brokers are adversaries | Fail |

**Tobias Reinhardt** (brought in for the gate): "Six fails. The interesting part is that the
product *works*. That's what makes it dangerous — it would generate enough revenue to keep us
busy for three years and never become a company."

**Decision: kill OFFMARKET as a business.** Keep the design pattern as an internal asset
([succession-deal-radar](../succession-deal-radar/SKILL.md), retained in this repo).

### 5b. What survived the kill

Three things from the failed thesis are load-bearing and were kept:

1. **The demographic engine is real and it is not a trend.** 2.3–3M boomer-owned US firms must
   change hands this decade; ~70% have no formal succession plan. Owners age whether or not our
   startup works.
2. **The moment of maximum pain is not the search. It is day 30 after the close.** Every
   persona with operating experience said the same thing unprompted.
3. **Cal Whitmore is still the customer.** We had the right person and the wrong problem.

**Diego Ramirez-Hale:** "I've been on the inside of six of these. The business doesn't break
because the buyer overpaid. It breaks because on day 40 nobody knows why the Thursday route
starts on the west side, and the two accounts that made the numbers work quietly leave. The
knowledge was never in the system. It was in a 60-year-old man's head, and he's in Florida now."

**Jonas Weill:** "Say that again, because that's my charge-off curve. My defaults cluster at
months 6 through 18 — after the seller leaves and before the buyer has learned the business.
If you sold *that*, I would put you in front of every borrower I have, and I'd do it because it
protects my book. That's not a referral favor. That's underwriting."

### 5c. The direction change

| | OFFMARKET (killed) | UNDERSTUDY (adopted) |
|---|---|---|
| Object scored | A person's likelihood of exiting | A business's knowledge coverage |
| Sold to | Searchers, pre-close | New owners, at and after close |
| Bought with | Personal credit card | Deal proceeds / working capital in the loan |
| Success means | Customer leaves | Customer becomes an operating subscriber |
| Channel | Content only | ⚠ Originally "lenders, brokers, SBDCs (incentive-aligned)" — **withdrawn.** Content-led, direct-to-buyer |
| Network effect | Negative in-market | Positive: each engagement improves capture models |
| Consent | Absent by design | Signed by the owner, revocable, on-screen |

### 5d. UNDERSTUDY against the same gate

| Criterion | Threshold | UNDERSTUDY (modeled) | Verdict |
|---|---|---|---|
| Net revenue retention | ≥ 100% | 108–124% (subscription + repeat acquisitions) | Pass |
| Serviceable revenue | ≥ $150M | ~$1.4B at modeled volumes (§7) | Pass |
| Marginal cost per market | Near zero | National from day one — no per-county data | Pass |
| Network effect | Positive | Trade-specific capture playbooks compound | Pass |
| Legal object | Not a natural person | Business operating knowledge, with consent | Pass |
| Channel with aligned incentive | Exists | ⚠ Lender default-reduction **withdrawn** — no default problem exists to solve at 0.71%. Channel now unproven | **Downgraded to open** |
| Gross margin | ≥ 65% | 68–74% engagement / 86% subscription | Pass (thin) |

**Sunhee Cho:** "I can sign this, with three conditions." → all three were built into the
prototype: (1) signed consent with a 30-day revocation window, shown in-product; (2) an explicit
out-of-scope list — employee performance, health, family, personal finances; (3) provenance on
every captured fact — session, timecode, speaker.

**Priya Anand** (added at M3): "Add a fourth. The outgoing owner is often still a creditor via
the seller note and sometimes still an employee. Capture cannot become a performance record of
anyone. Put the guardrail in the interface where the buyer can see it fire."
→ **Incorporated:** the guardrail event is rendered in the capture view.

---

## 6. Why demand explodes — the mechanism, not the market size

Market size is not a demand mechanism. These four are:

1. **Contractual necessity.** Seller notes, earnouts, and transition periods already exist in
   most lower-middle-market deals — meaning the parties have *already agreed in writing* that
   knowledge must transfer. Today that obligation is discharged with "call me if you have
   questions." We are the instrument that discharges it.
2. ⚠ **WITHDRAWN — "an underwriter's financial interest."** The original claim was that lender
   defaults cluster in months 6–18 and a lender would therefore require us. Acquisition loans
   default at ~0.71% with a 4.1-year median. **No demand multiplier exists here.** What replaces
   it: nothing yet. The revised plan (MEETING-MINUTES.md §4) treats distribution as unsolved and
   builds technical advantage first rather than assuming a channel.
3. **Payment timing.** Our fee is spent from closing proceeds, at the one moment in the
   customer's life when capital is allocated and a wire is already going out. We are a line on
   a closing statement, not a subscription he has to re-justify each month.
4. **A capability that arrived, not a preference that shifted.** A 66-year-old will talk for
   22 minutes on the phone and will never type into a wiki. Voice capture plus structured
   extraction became cheap enough to make talking the interface in the last 18 months. The
   demand was always there; the instrument wasn't.

**Aisha Bello:** "And the content writes itself: 'what the last owner knew.' Every episode is a
real business, a real gap, and a real number. That's the same engine I wanted at OFFMARKET,
pointed at a customer who doesn't leave."

---

## 7. Business model and unit economics (modeled)

**Two lines, deliberately:**

- **Handover engagement** — $14,500 typical (band $9K–$28K, scaled to deal size, ~0.4–0.8% of
  enterprise value). 90 days, ~24 capture sessions, delivered prompt book.
- **Operating subscription** — $590/mo base + $40/seat beyond 5, starting at day 91.

**Modeled engagement economics**

| Line | Modeled |
|---|---|
| Price | $14,500 |
| Agent + infrastructure cost | $900 |
| Human QA (7.5 hrs @ $85 loaded) | $640 |
| Owner incentive (paid to the seller for their time) | $1,500 |
| Channel referral fee | $1,450 |
| **Gross margin** | **~71%** |

**Tobias Reinhardt:** "71% is acceptable and it is *fragile*. The number that kills us is QA
hours per engagement. If that goes to 20 hours we're a consultancy with a website. I want it
instrumented from engagement one and reported at every board meeting."
→ **Incorporated as a tracked kill metric** (§9).

**Five-year path (modeled, not projected revenue)**

| Year | Engagements | Subscribers (exit) | Modeled ARR-equivalent |
|---|---|---|---|
| 1 | 40 | 32 | $0.8M |
| 2 | 180 | 170 | $3.8M |
| 3 | 520 | 520 | $12.2M |
| 4 | 1,300 | 1,450 | $32M |
| 5 | 2,800 | 3,400 | $74M |

Sanity check on the ceiling: at ~200K annual US small-business ownership transitions with any
formal transition period, a 1.5% share at this price band is roughly $1.4B of engagement revenue
plus recurring. Year 5 above assumes **0.14% share.** The plan does not require winning the
market; it requires not stopping.

---

## 8. Meeting 3 — Prototype review (end of M3)

The three views were built and reviewed by the full cast plus customer personas.

**Diego Ramirez-Hale:** "The crew view is the only screen I believe. A tech asks out loud and
gets Bud's actual voice — that's adoption without training. But your first two screens are for
the buyer, and the buyer isn't the hard user. Bud is."
→ **Incorporated:** the capture session view now shows Bud's own words as the primary typography
(serif, largest text on the screen) and the agent's questions as secondary. The owner is the
author of the record, not its subject.

**Halina Novak:** "22 minutes is the ceiling and you've honored it. One correction: never open
with the highest-risk gap. Open with something he's proud of. Warm-up is not wasted time, it's
recall quality. Also — 'Bud confirms' as a button label is right. Confirmation must be *his*
act, not our inference."
→ **Incorporated:** session agenda holds 4 slots, not 6; confirmation is an explicit act
attributed to the owner; a warm-up slot is reserved and not fillable from the gap list.

**Bud Kessler** (owner persona): "First thing I want to know isn't on there. Does the crew keep
their jobs? Does my name come off the trucks? Show me *that* before you ask me about boilers."
→ **Incorporated as a product requirement, deferred to build 2:** an owner-facing view opening
with the buyer's written commitments on name, crew, and customers. Flagged in §10 — this is the
single largest gap in the current prototype.

**Cal Whitmore** (buyer persona): "61% — is that good or bad? I need to know what number means
I'm safe, and I need to be able to hand a lender something."
→ **Incorporated:** coverage is weighted by revenue exposure rather than page count, and the
"if Bud stops answering tomorrow" panel converts coverage into dollars, days, and minutes owed.
A benchmark band ("safe ≥ 85% by day 90") is queued for build 2.

**Denise Okafor** (lender persona): "I don't want your dashboard. I want one page per borrower,
monthly, that tells me whether the transition is on track — and I want it in the file. Build me
a report, not a login."
→ **Incorporated as the primary sales artifact:** the lender deliverable is a one-page monthly
continuity report, not a seat. Reflected in the proposal.

**Sunhee Cho:** "Guardrail is visible. Provenance is on every card. Revocation is stated.
Signed."

**Ramona Fitzgerald** (SBDC persona): "For public money I need jobs retained per business,
per quarter. Your coverage number is interesting to a buyer and useless to me."
→ **Deferred with a date** (§10): a B2G outcome report is a Year-2 item, not a Year-1 dilution.

**Rin Takeda:** "Two things I refused. No donut charts — coverage is a composition, so it's a
spine of eight segments weighted by revenue exposure. And no green-means-good: the only colored
things on the screen are risks. Calm is the absence of color."

---

## 9. Risks and kill criteria

| Risk | Severity | Mitigation | Kill criterion |
|---|---|---|---|
| QA hours per engagement creep | **Highest** | Instrument from engagement 1; trade-specific extraction templates | >14 hrs average at engagement 50 → re-price or stop selling |
| Owners refuse to be recorded | High | Owner incentive payment; revocation window; owner-first framing (build 2) | <55% owner consent rate across first 30 deals |
| Engagement doesn't convert to subscription | High | Crew view live before day 90 so the habit forms pre-renewal | <45% day-91 conversion at n=50 |
| ⚠ ~~Lender channel doesn't materialize~~ | — | **Resolved by being wrong.** The channel had no economic basis; withdrawn before any effort was spent | Closed |
| **No proven channel at all** | **Highest, replacing the above** | Content is the only channel needing no external party; sequenced after the V3 engine test | No repeatable acquisition path by month 9 post-V3 |
| Elicitation advantage doesn't exist | **Existential** | Formal synthetic benchmark, ground truth sealed before the engine is written | **K1:** treatment fails 1.4× CRR *and* 3× ERR → stop |
| Mechanic commoditized by consumer products | Medium | Never lead with capture; lead with ranking. Moat is T1/T2/T3 | Competitor ships consequence-ranked elicitation first |
| FSM incumbent bundles this | Medium | The founder's voice archive is not reproducible after the owner leaves; we are the system of record for the *past* | — |
| Services-margin trap | Medium | Hard 65% GM floor per engagement | Two consecutive quarters <65% |

**Honest statement of the weakest point:** this business is one metric away from being a
consultancy. Everything durable about it — the margin, the scalability, the brand — depends on
capture staying agent-led with humans only in QA. That is the number to watch, and we have said
so on the record rather than discovering it in year three.

---

## 10. What is not built yet

1. **Owner-first onboarding view** (Bud's ask) — the largest gap. Build 2.
2. **Coverage benchmark band** — "what number means I'm safe." Build 2.
3. ⚠ ~~**Lender monthly report**~~ — dropped with the channel.
4. **B2G outcome reporting** — jobs retained per business. Year 2.
5. Live voice pipeline, retention/deletion tooling, seller-note milestone integration.
6. **V1–V3: the HVAC ontology, the elicitation policy engine, and the synthetic-owner benchmark.**
   This is now the top of the queue — it tests whether the company has a reason to exist.
   Specification in [MEETING-MINUTES.md](MEETING-MINUTES.md) §5.

---

## 11. Prototype

`demo/index.html` — three views, no build step, no external requests.

1. **Prompt book** — continuity coverage weighted by revenue exposure, eight operating domains,
   ranked gaps with the money each one exposes, and a session agenda you assemble from the gaps.
2. **Capture session** — the outgoing owner's own words as the primary type, extracted facts
   awaiting *his* confirmation, full provenance, and a visible guardrail event.
3. **Crew view** — the same knowledge one day later, on a phone, answered in the owner's voice.

Design pattern documented in [SKILL.md](SKILL.md).
