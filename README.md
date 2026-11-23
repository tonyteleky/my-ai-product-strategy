# AdQuest | AI Product Strategy

> **Product School capstone · Tony Teleky**  
> AdQuest helps local TV sellers decide which advertisers to pursue next by turning proprietary advertising data into a ranked prospect list with dated evidence and a recommended next action.

**Decision requested** — Approve a capped **$50,000, 12-week pilot** for up to 20 local TV sellers. Release $20,000 for the first four weeks and the remaining $30,000 after an evaluation, permissions, and operational readiness review. The budget and financial model are planning assumptions. The pilot will test customer value, reliability, and economics before expansion.

---

## Strategy at a Glance

| Component | Module | Status | Key Artifact |
|-----------|--------|--------|-------------|
| **The Bet** | M1 | [x] | `01-the-bet/` |
| **The Moat** | M2 | [x] | `02-the-moat/` |
| **The Margin** | M3 | [x] | `03-the-margin/` |
| **The Contract** | M4 | [x] | `04-the-contract/` |
| **The Guardrails** | M5 | [x] | `05-the-guardrails/` |
| **The Pitch** | M6 | [x] | `06-the-pitch/` |

---

## The Bet (M1)

- **Product** — AdQuest's Combined AI Strategy Agent starts with local TV seller prospecting. Sellers already have market and advertiser data, yet still spend time turning it into outreach priorities. The pilot tests whether sourced recommendations shorten that work. Buyer planning is a later expansion.
- **AI value archetype** — Oracle first, using market and competitive data to surface opportunities. Copilot second, translating those signals into next actions a seller can review.
- **Vulnerability scores** — Contextual moat **3/5** · Data advantage **4/5** · Platform exposure **5/5**, as scored in the M1 diagnostic.
- **Top risk** — Workflow depth. A vertical competitor with comparable data could win the seller's day-to-day prospecting workflow.
- **Confidence** — **High** in the original M1 diagnostic. **Medium** for the scoped H1 pilot in the M6 roadmap.
- **Prototype** — [AdQuest advertising intelligence demo](https://github.com/user-attachments/files/33983520/index.html).
- **Kill criteria** — Stop expansion if fewer than **30%** of pilot sellers take a documented action on a recommendation or median research time falls by less than **20%** versus comparable manual tasks by week 8. Evidence must be recent and verifiable enough for sellers to act.

→ Details: [`01-the-bet/`](01-the-bet/)

---

## The Moat (M2)

- **Data flywheel** — **9/20**. Correction **2/5**, preference **2/5**, domain context **4/5**, and network **1/5**. Network is the weakest loop. Existing feedback reaches the backlog and gives the team a starting point for reviewed regression cases.
- **Competitive position** — On proprietary advertising-data depth and integration into seller workflows, AdQuest's strongest position today is data depth: historical coverage, collection, classification, and estimation. MediaRadar is the closest vertical threat. A general-purpose platform could close the data gap through a licensing partnership.
- **Encroachment defense** — Show the evidence behind each recommendation, make verified corrections reusable, and embed reviewed next actions in sellers' reporting and CRM workflows.
- **Vendor portability** — **Partial** Demonstrate a provider switch and rollback within **48 hours** that passes quality and data-policy checks before relying on a backup.

→ Details: [`02-the-moat/`](02-the-moat/)

---

## The Margin (M3)

- **Gross margin** — Modeled traditional SaaS baseline **80.0%**. Base subscription with bundled AI **72.0%** at 400 requests per user per month and $0.02 blended inference cost. At five paid plans per month, modeled margin is **81.1%** ($150 revenue and $28.40 COGS). At 20% premium adoption with five plans per premium user, modeled cohort margin is **74.5%**. Incremental AI infrastructure, storage, and review costs still need estimates.
- **Pricing** — **$100 per seat per month** for core analytics and lightweight AI, plus **$10 per completed premium strategy plan**.
- **Model routing** — Target **60% small / 20% mid-tier / 20% frontier**. Small models handle routine requests, mid-tier models handle competitive analysis, and frontier models handle complex forecasting and multi-step plans as needed.
- **Break-even** — One paid plan per seat per month offsets the modeled $8 in bundled inference and that plan's incremental inference cost, restoring baseline gross profit per seat. Five plans restore the modeled 80% SaaS margin. The pilot will measure fully loaded cohort margin against a **65%** threshold.

→ Details: [`03-the-margin/`](03-the-margin/)

---

## The Contract (M4)

- **Proposed reliability gates** — **≥92%** of cases pass the full rubric, **100%** pass critical budget, inventory, and authorization checks, and **<1%** of evaluated plans contain unsupported material factual claims. Target **p95 <15 seconds** for completed plans and **≤0.5 percentage-point** accuracy decline over four weeks.
- **Golden dataset** — **11 synthetic starter cases**, including **4 adversarial** cases. Expand toward **150 reviewed cases** before v1. Apply deterministic checks for limits and access, plus a human-calibrated judge for evidence and actionability.
- **Confidence and human review** — Label observed facts, inferences, and verified commercial conditions. Show dated sources and assumptions. Ask for clarification or route to an analyst when material evidence is missing, disputed, or low confidence. Users approve external sharing and other consequential actions.
- **Failure modes** — Stale or missing data, hallucinated budgets, unsupported purchase intent or inventory claims, performance guarantees, prompt injection, and unauthorized disclosure. A critical failure immediately disables the affected capability.

→ Details: [`04-the-contract/`](04-the-contract/)

---

## The Guardrails (M5)

- **Compounding system** — Product and data teams triage feedback weekly, verify corrections, add regression cases, and test fixes before release. Track repeat errors and correction-to-fix time. Evaluate cross-workflow improvements on held-out cases before claiming they transfer.
- **Governance and agent boundaries** — Check permissions before retrieval, isolate confidential account data, and use approved providers and logged tools. AI can retrieve authorized data, calculate, and draft. Users approve saves, exports, sharing, and connected-system changes. Ad purchases, budget commitments, campaign changes, and contractual promises stay with authorized people.
- **Shadow AI** — **0 confirmed** external workarounds. **5 hypotheses provisionally triaged** as two build, two partner, and one monitor. Customer interviews and support evidence will validate frequency and intent.
- **Regulatory exposure** — Legal and security review privacy and AI obligations, advertising-data licenses, customer agreements, and provider terms before launch. EU AI Act applicability and risk classification are pending review of intended use and markets.

→ Details: [`05-the-guardrails/`](05-the-guardrails/)

---

## The Pitch (M6)

**How you get this funded, shipped, and adopted.**

| Horizon | Investment | Gate |
|---------|------------|------|
| **Now · 0–3 months** | Pilot seller prospecting, build the evaluation and feedback process, and test paid plans. | By week 8, **≥30%** take a documented action and median research time falls **≥20%**. Before broader release, meet reliability gates. By week 12, **≥20%** of at least 10 eligible users buy a plan and fully loaded cohort gross margin reaches **≥65%**. |
| **Next · 3–9 months** | Add explicit account preferences, approved CRM workflows, and a backup provider for prospecting. | Reduce repeat errors **≥20%** on a frozen test set, reach **≥40%** weekly CRM saving among participants, and demonstrate a safe provider switch and rollback within **48 hours**. |
| **Bet · 9–18 months** | Test buyer planning with authorized inventory and pricing. Evaluate privacy-reviewed learning across workflows. | Reduce buyer planning time **≥20%** while passing all critical checks. Demonstrate a **≥5 percentage-point** rubric improvement on a held-out workflow without critical regressions or confidential-data exposure. |

- **Board Narrative:** — Fund a focused seller pilot to prove that AdQuest's proprietary advertising intelligence can drive measurable action, then expand only when reliability, paid adoption, and delivery costs support it.

- **Key metric** — The share of pilot sellers who take a documented action on an AdQuest recommendation by week 8, with a **30%** target.

→ Details: [`06-the-pitch/`](06-the-pitch/)
