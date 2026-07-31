# Strategy Planning Meeting — Minutes

**Meeting:** M5 · Direction of service implementation
**Date:** 30 July 2026
**Chair:** Ye-jin Park (Founder)
**Input:** [MARKET-RESEARCH.md](MARKET-RESEARCH.md)
**Standing constraints imposed by the principal:**
1. Pivot to UNDERSTUDY accepted — no re-litigation.
2. **No external resources.** The plan may not assume partners, capital, hires, or introductions.
3. **Priority is bargaining power through technical barriers**, not market access.
4. HVAC first.

---

## Attendees

**Internal (10):** Ye-jin Park (CEO) · Marcus Oyelaran (Data) · Sunhee Cho (Trust & Compliance) ·
Diego Ramirez-Hale (Field Ops) · Aisha Bello (Growth) · Jonas Weill (Capital Partnerships) ·
Rin Takeda (Design) · Halina Novak (Voice & Extraction) · Tobias Reinhardt (CFO) ·
Priya Anand (Counsel)

**Customer personas present (4):** Cal Whitmore (buyer) · Bud Kessler (outgoing owner) ·
Denise Okafor (lender) · Ramona Fitzgerald (SBDC)

**External expert advisory panel — newly convened (6):**

| Advisor | Standing | Why they are in the room |
|---|---|---|
| **Dr. Ingrid Sæther**, 54 | Cognitive task analysis researcher; 20 years of knowledge-elicitation fieldwork in aviation maintenance and nuclear operations | The only person here who has professionally extracted expertise from an unwilling expert |
| **Kenji Morishita**, 61 | 事業承継 advisor, Nagoya; 300+ SMB successions through Japan's public support network | Has already lived through the market we are forecasting |
| **Seo-yeon Lim (임서연)**, 45 | 세무사 / 가업승계 practice; advises Korean manufacturing SMEs on succession and 가업상속공제 | Knows where a fee can and cannot sit in a Korean succession |
| **Dr. Adebayo Ncube**, 39 | Speech AI; far-field ASR and elderly/dysarthric speaker adaptation | Owns the one technical claim we can test alone |
| **Rachel Kwon**, 48 | Ex-VP Product, connected-worker platform ($60M ARR, manufacturing) | Has shipped the enterprise version of our product and knows why it stops at the enterprise |
| **Tomás Beltrán**, 57 | Master HVAC technician, 31 years; ran a 14-truck shop, sold it in 2021 | Is Bud, and can tell us when we are wrong about Bud |

---

## 1 · Research readout (Ye-jin, 12 min)

Three findings placed on the table without softening:

1. Our square (transition-moment knowledge capture for SMB ownership transfer) is **empty in
   Korea, Japan, and the US.**
2. Our **mechanic is already commodity** — Tell Mel runs AI biographer phone calls with no app
   and no typing; Remento ships QR-to-original-voice.
3. **The lender thesis is dead.** SBA acquisition loans default at 0.71%, the lowest of any 7(a)
   purpose, with median time to default of 4.1 years.

**Jonas Weill:** "That third one is mine and it's wrong, so let me be the one to say it. I gave
you a pattern from memory and you built a customer proposal on it. Twenty years in credit and I
would have sworn to the months 6-to-18 cluster. The portfolio data says 4.1 years. Withdraw the
channel."

**Chair's ruling:** lender-first channel **withdrawn**. Proposal re-pointed at the buyer. The
correction is recorded in the research document against our own interest, not buried.

---

## 2 · The commodity problem (30 min)

**Rachel Kwon** opened, and reframed the meeting: *"You are describing yourselves by your input.
Everyone in my old category did that too — 'we capture tribal knowledge on video.' Then Dozuki
shipped CreatorPro, and everybody's demo looked the same in a quarter. Capture is a feature. What
never commoditized for us was knowing **which** ten minutes of a forty-year career were worth
recording. We never solved that. We shipped a camera and told the customer to point it."*

**Dr. Ingrid Sæther:** *"That is the entire discipline of knowledge elicitation and you are
treating it as an afterthought. An unstructured interview with an expert recovers surface
procedure — what they can already tell you. The valuable knowledge is the exception handling, and
experts do not volunteer exceptions because to them the exception is obvious. You have to ambush
it: present a degraded case and ask what they would do. Your product asks 'tell me about
pricing.' A trained elicitor asks 'the Mercy Clinic contract renews in October at the handshake
rate — what happens if the new owner sends a standard rate sheet?' Those two questions do not
recover the same knowledge, and the difference is not small. It is the difference between the
80% that is already written down and the 20% that isn't."*

**Tomás Beltrán:** *"She's right and I'll tell you exactly how. If you'd called me in 2021 and
asked what a new owner needs to know, I'd have talked for twenty minutes about equipment. Totally
useless — that's in the manuals. Nobody asked me the thing that actually mattered, which is that
Kaiser's facilities manager and I had a deal about after-hours calls that wasn't in any contract,
and when I left, my buyer billed them overtime and lost the account in five months. That's
$180,000 a year that walked because nobody knew to ask one question."*

**Halina Novak:** "That is our metric, then. Not minutes recorded. **Dollars of exposure retired
per question asked.**"

**Decision D1 — identity restated.**
> We are not a capture company. **We are a targeting company that happens to capture.**
> Every external description of the product leads with ranking, never with the microphone.

---

## 3 · Where the technical barrier actually is (45 min)

Marcus and Dr. Ncube separated what is defensible from what is table stakes.

| Layer | Defensible? | Reasoning |
|---|---|---|
| ASR / transcription | ❌ | Commodity. Multiple vendors, near-zero switching cost |
| LLM extraction into structured facts | ❌ | Commodity within 12 months |
| Voice playback of the original speaker | ❌ | Remento shipped it to consumers |
| Scheduled AI phone interview | ❌ | Tell Mel shipped it to consumers |
| **T1 · Elicitation policy — the question graph** | ✅ **Strongest** | Given a coverage state and a trade, which single question retires the most exposure. Compounds with every engagement. Not derivable from public data |
| **T2 · Consequence model** — knowledge unit → revenue exposure | ✅ **Strong** | Requires outcome-labeled data nobody has. Two years of engagements makes it unassailable |
| **T3 · Verification ledger** — owner confirmation as the only write path, crew queries as reward signal | ✅ **Structural** | A closed loop competitors cannot retrofit without the same data |
| **T4 · Trade-jargon speech adaptation** | ⚠ **Temporary** | Real for 18–24 months, then eroded by general models |
| **T5 · Consent, provenance, refusal architecture** | ✅ **Regulatory** | Cheap now, expensive to retrofit. Korea's policy gap makes it strategic |

**Dr. Adebayo Ncube:** *"T4 is real but do not build a company on it. A 66-year-old in a truck
bay with a diesel idling — general ASR degrades badly on that, and 'Weil-McLain' and 'aquastat'
and 'Taco zero-oh-seven' are not in anyone's language model. Lexicon biasing per trade buys you a
genuine accuracy gap today. It buys you eighteen months. Take the eighteen months, and spend them
building T1, because T1 does not erode."*

**Sunhee Cho on T5:** *"Korea's own tacit-knowledge programme has publicly admitted that
contributor IP and compensation are unresolved. We already pay the owner and we already log
provenance. If Korea writes a rule, we are the reference implementation instead of the
retrofit. That is worth building before anyone asks for it."*

**Decision D2 — the moat, in order.**
> **T1 elicitation policy** is the company. **T2 consequence model** is its compounding asset.
> **T3 verification ledger** makes both non-copyable. **T4** is an 18-month tactical advantage,
> deliberately taken. **T5** is cheap insurance that may become the licence to operate in Korea.

---

## 4 · Geography (18 min)

**Kenji Morishita:** *"Japan will validate your thesis and destroy your company. 24,000
consultations a year through the public centres, BATONZ listed this year, 技能継承くん and 匠AI
already selling AI tacit-knowledge capture. Every one of those relationships took a decade. You
would be a foreign startup with no 紹介. Come to Japan in year four with proof, not in year one
with a demo."*

**Seo-yeon Lim:** *"Korea is more interesting than you think, but not for the demographics. 675,000
SMEs with an owner over sixty and no successor — yes. The real point is where your fee sits. In a
Korean succession the money moves through 가업상속공제 and the tax structure, and there is no line
on the closing where a $14,500 knowledge fee naturally lands. You would have to create that line,
which means educating 세무사 and 회계법인 — external people, which you are currently forbidden from
recruiting. Korea is your best strategic market and your worst first market. Precisely because
of the constraint."*

**Decision D3 — geography deferred, deliberately.**
> Build the engine **domain-first, geography-agnostic.** Verify on a US HVAC ontology because the
> trade vocabulary is public and abundant, not because the US is the chosen beachhead. Korea and
> Japan are re-evaluated only when the engine clears its numeric gate. **Choosing a geography now
> would require exactly the external relationships we are barred from assuming.**

---

## 5 · Verification protocol under zero external resources (40 min)

**Cal Whitmore:** "You still haven't proven anyone pays."
**Chair:** "Correct, and under the current constraint we cannot. So we are not going to pretend.
We verify the one claim that is testable alone: that targeted elicitation recovers more
consequential knowledge per minute than a competent generic interview. If that is false, there is
no company, and no amount of customer access would save it."

### V1 · HVAC knowledge ontology
Build ~8 domains × ~120 knowledge units from public sources — trade manuals, licensing curricula,
code requirements, public forum threads, equipment documentation. Each unit tagged with an
exposure class. **Owner:** Marcus. **Output:** a versioned ontology file.

### V2 · Elicitation policy engine
Given a coverage state, emit the next question. Scoring: `expected exposure retired × recall
probability ÷ expected answer length`. **Owner:** Halina + Sæther as reviewer.

### V3 · Synthetic-owner benchmark — the core experiment
A simulated owner holds a **hidden ground-truth knowledge set** (~140 units, exposure-weighted,
deliberately including exceptions the owner will not volunteer). Two interviewers run 22-minute
sessions against it:
- **Baseline:** a competent generic AI interviewer ("tell me about your pricing").
- **Treatment:** our elicitation policy.

Measured over 12 simulated sessions:

| Metric | Definition | Gate |
|---|---|---|
| **CRR** Coverage Recovery Rate | Exposure-weighted % of ground truth recovered by session 12 | Treatment ≥ **1.4×** baseline |
| **QTC** Questions-to-Coverage | Questions needed to reach 60% exposure coverage | Treatment ≤ **0.6×** baseline |
| **ERR** Exception Recovery Rate | % of non-volunteered exception units recovered | Treatment ≥ **3×** baseline |
| **FPR** False-fact rate | Extracted facts not in ground truth | < **2%** |

> **Kill criterion K1:** if treatment fails to beat baseline by 1.4× CRR *and* 3× ERR, the
> elicitation thesis is wrong and the company stops. No pivot, no second attempt with a bigger
> prompt. Stop.

**Dr. Sæther's condition, accepted:** *"Your ground truth must be built by someone other than
whoever writes the policy engine, or you will grade your own homework. And put in the exceptions
the expert would never mention. If your hidden set is only surface procedure, both arms score
well and you will have learned nothing."*
→ **Incorporated:** ground truth authored and sealed before the policy engine is written; ≥40% of
units classed as non-volunteered exceptions; Tomás Beltrán reviews the HVAC set for realism.

### V4 · Jargon lexicon accuracy
Build the HVAC lexicon (brands, part numbers, trade slang) and measure extraction accuracy on
jargon-dense transcripts. **Stated limitation, not to be papered over:** synthetic transcripts do
not test acoustics. Real-world WER on a 66-year-old in a noisy bay is **unverifiable without
recording a real person**, and remains an open risk until the constraint lifts.

**Decision D4 — verification sequence:** V1 → V2 → V3 → V4, gated at V3. Nothing is built beyond
the prototype until V3 clears.

---

## 6 · External expert capability specification

Requested explicitly. For each capability: what it must be, why it blocks us, what we substitute
today, and how a candidate is tested.

| # | Capability required | Blocks | Substitute under the constraint | Screening test |
|---|---|---|---|---|
| **E1** | **Knowledge elicitation / cognitive task analysis.** Must have run structured elicitation with hostile or indifferent experts; must know critical-decision and PARI-style methods by name and limitation | **T1 — the moat itself** | Published CTA literature; Sæther persona as reviewer | "An expert says 'you just get a feel for it.' Give me your next three questions." A weak candidate rephrases the question; a strong one degrades the case |
| **E2** | **Trade master (HVAC, 25+ yrs, ran a shop).** Ground-truth validator and exception source | **V1/V3 validity** | Public trade curricula and forums; Beltrán persona | Hand them 20 extracted facts. Strong candidates immediately separate "in every manual" from "cost me money to learn" |
| **E3** | **Speech AI — far-field, elderly, domain lexicon.** Must have shipped lexicon biasing and measured WER by speaker age | **T4, and all real-world capture** | Domain lexicon built in-house; acoustics untested | "WER on speakers 65+ versus your headline number, and how did you close it?" No age-stratified answer = no capability |
| **E4** | **Privacy counsel — Korea PIPA and US state regimes.** Must be fluent in consent withdrawal, retention limits, and the status of a recording of a person who is also a creditor | **T5, and launch in Korea** | Conservative design already shipped: signed consent, 30-day revocation, out-of-scope list, provenance | "Our subject is the seller, an employee, and a creditor at once. Whose record is the recording?" |
| **E5** | **Succession practitioner — KR 세무사 / JP 承継 advisor.** Must know exactly where a fee lands on a closing | Geography entry, pricing | Deferred with D3 | "Show me the line our fee sits on in a 가업승계 closing." Vagueness disqualifies |
| **E6** | **SMB trades go-to-market operator.** Sold software into sub-30-employee trade businesses | Post-verification revenue | Deferred until after V3 | "Describe your last five losses." No specific loss stories = no field time |

**Decision D5 — hiring order, when the constraint lifts:** E1 first — it is the moat, and it is
the one capability we cannot fake from literature indefinitely. E2 next, cheaply, as paid
advisory. E3 when real audio exists. E4 before any Korean pilot. E5 and E6 only after V3 clears.

**Tobias Reinhardt:** *"And note what this list is not. There is no head of sales, no partnerships
lead, no data broker. Every capability on this list makes the engine better. That is what
building bargaining power actually looks like — when you finally talk to a lender or a 세무사,
you want to be arriving with something they cannot get elsewhere, not asking for a favour."*

---

## 7 · Objections recorded and unresolved

Not decisions. Things the meeting could not settle, kept visible.

1. **Bud Kessler:** *"Nobody in this room has asked a real 66-year-old if he'll do this. You've
   got a simulated me now. I'm flattered, but I'm not evidence."* — Correct. Consent rate remains
   the largest unvalidated assumption and cannot be tested under the current constraint.
2. **Ramona Fitzgerald:** *"Your synthetic benchmark can't produce a jobs-retained number, so
   public money still can't buy you."* — Accepted. B2G remains year 2+.
3. **Rachel Kwon:** *"When you clear V3, the enterprise vendors can read your marketing and copy
   the idea. Your protection isn't the idea — it's T2, and T2 needs real engagements. There is a
   window where you are copyable, and the constraint you're operating under makes it longer."* —
   Recorded. No mitigation exists that does not require customers.
4. **Aisha Bello:** *"Content is the one channel that needs no external anyone. Every V-step
   produces a publishable artifact. Let me publish the benchmark, including if it fails."* —
   Approved in principle; sequenced after V3 so we publish a result rather than a promise.

---

## 8 · Conclusions

1. **Identity:** a targeting company that happens to capture. Never led by the microphone.
2. **Moat:** T1 elicitation policy → T2 consequence model → T3 verification ledger.
   T4 taken as an 18-month advantage. T5 built now as cheap insurance and possible Korean licence.
3. **Lender channel:** withdrawn on the data. Proposal re-pointed at the buyer.
4. **Geography:** deferred by design; engine built domain-first, verified on US HVAC vocabulary.
5. **Next work:** V1 → V2 → V3, gated. Kill criterion K1 is binding.
6. **External experts:** six capabilities specified, ranked, with substitutes and screening tests.
   None are required before V3, which is what makes the plan executable under the constraint.
7. **Honest position:** we have proven the square is empty and the mechanic is commodity. We have
   proven nothing about whether the engine works or anyone pays. V3 addresses the first.
   The second stays open until the no-external-resources constraint lifts, and we will not
   pretend otherwise in any document that leaves this room.
