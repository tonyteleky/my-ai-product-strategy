# Three-Horizon Roadmap & Board Pitch

**Product:** AdQuest — Combined AI Strategy Agent

## Roadmap

### Horizon 1 — Now (0-3 months)
*Quick wins. Ship with existing capabilities.*

| Initiative | Metric | Confidence |
|-----------|--------|-----------|
| Pilot evidence-backed advertiser prospecting with local TV sellers using existing advertising data. Show prioritized prospects, supporting evidence, and recommended next actions. | In a pilot of up to 20 sellers, ≥30% take a documented action on a recommendation and median research time falls ≥20% versus comparable manual tasks. Stop expansion if either threshold fails by week 8. | M |
| Establish a verified feedback-to-improvement process using existing Ask AdQuest feedback. Add source dates, evidence labels, and regression tests for known failures. | Expand the 11-case starter dataset toward 150 reviewed cases; achieve ≥92% rubric pass rate and 100% pass rate on critical budget, inventory, and authorization checks before broader release. | M |
| Test hybrid pricing and measure actual delivery costs. | By week 12, ≥20% of at least 10 eligible users purchase a $10 strategy plan, with ≥65% fully loaded pilot-cohort gross margin. If either threshold fails, revise packaging or scope before expanding paid access. | M |

### Horizon 2 — Next (3-9 months)
*Bets. Requires new capabilities or integrations.*

| Initiative | Metric | Confidence |
|-----------|--------|-----------|
| Add explicit account preferences and reusable, human-validated corrections to improve recommendations over time. | Within an eight-week experiment, reduce repeat errors ≥20% on a frozen evaluation set without critical regressions. If two tested releases produce no improvement, stop personalization expansion and prioritize data/retrieval fixes. | M |
| Connect approved CRM workflows so users can review and save prospecting recommendations where they work. | Within eight weeks of pilot access, ≥40% of participating users save an approved recommendation to their CRM at least weekly. If usage stays below 20%, stop additional connector investment. | M |
| Validate a provider-neutral model interface and backup-model path for the initial seller workflow. | Demonstrate a safe switch and rollback within 48 hours while maintaining release quality and data-policy requirements. If the backup fails those checks, do not activate it or claim portability readiness. | M |

### Horizon 3 — Bet (9-18 months)
*Moonshots. High uncertainty, high potential.*

| Initiative | Metric | Confidence |
|-----------|--------|-----------|
| Extend the agent into buyer media planning using authorized inventory, pricing, and audience data. | In an eight-week experiment with at least five buyer design partners, reduce median planning time ≥20% while passing all budget, inventory, and authorization checks. Stop if current, authorized data are unavailable or value targets fail. | L |
| Test whether privacy-reviewed, de-identified corrections improve recommendations across advertising workflows. | Improve rubric pass rate ≥5 percentage points on a held-out second-workflow dataset, with no critical regressions or confidential-data exposure. Stop the experiment if privacy controls fail or no improvement appears within six weeks. | L |

**Sequencing principle:** H1 must demonstrate customer value, reliability, and sustainable delivery costs before H2 expansion. H3 requires a separate investment decision supported by evidence.

## Board Pitch

**Thesis (1 sentence):**
AdQuest will help local TV sellers turn advertising intelligence into evidence-backed prospecting actions, starting with a bounded pilot that must prove time savings, customer adoption, and sustainable economics.

**The case:**
1. Why now: This advances AdQuest’s core purpose: helping customers use advertising intelligence to make better decisions. We already have specialized data, reporting workflows, and an AI feedback surface; the next step is to test whether those assets shorten sellers’ research-to-action workflow. The timing case rests on those existing capabilities, not a verified external market change. Start with seller prospecting and earn the right to expand.

2. What's defensible: Our M2 assessment identifies proprietary advertising collection, historical coverage, classifications, estimation methodology, and domain context as the advantage. Competitors can copy the interface; reproducing the underlying data operations and analytical context is harder. However, our flywheel scores only 9/20, with network effects at 1/5. We will strengthen workflow depth through verified corrections and explicit account preferences, and claim compounding only when measured improvements support it.

3. The economics: $8 per user per month is the modeled routine inference cost at 400 requests. Proposed pricing is $100 per seat plus $10 per completed premium strategy plan. Five paid plans produce 81.1% modeled gross margin for a premium user; at 20% premium adoption, modeled cohort margin is approximately 74.5%. Both exclude unestimated incremental infrastructure, storage, and review costs. In the fixed-$100 base scenario, tripling inference costs reduces modeled margin from 72% to 56%. Routing and caching are proposed controls, not demonstrated savings. The pilot must validate actual payment and at least 65% fully loaded cohort gross margin.

**The risks:**
1. Trust / failure modes: The most consequential failure is disclosing another customer’s confidential data or presenting an inferred opportunity as confirmed buying intent, available inventory, or guaranteed performance. Enforce permissions before retrieval, distinguish observed facts from inferences and verified conditions, and show dated sources. Before broader release, expand the 11-case starter dataset toward 150 reviewed cases and require ≥92% rubric pass rate, 100% critical hard-check compliance, and <1% unsupported-material-claim rate. Critical failures immediately disable the affected capability; these controls reduce risk but do not guarantee detection of every failure.

2. Scale / governance: At 10x usage, analyst review demand, latency, and delivery costs could undermine the business case. Track review minutes, cost per completed plan, retries, and quality by workflow before increasing access. Product and data teams validate corrections and test fixes before release. Confidential account data remain isolated, and users approve saves, exports, sharing, and connected-system changes. The agent cannot purchase ads, commit budgets, change campaigns, or make contractual promises. Provider portability remains unproven until a tested switch and rollback passes quality and data-policy checks.

3. Competitive: The scenario most likely to undermine this bet is a vertical competitor such as MediaRadar pairing comparable intelligence with a more useful seller workflow. We will judge our response through customer behavior rather than feature parity. Stop expansion if fewer than 30% of pilot sellers act on a recommendation or research time falls by less than 20% by week 8. If paid conversion remains below 20% or fully loaded cohort margin falls below 65% at week 12, stop rollout at the proposed packaging and revise the offer.

**The ask:**
Approve a capped $50,000, 12-week pilot for up to 20 local TV sellers: one dedicated engineer, 0.25 PM, 0.25 data analyst, and fractional security and commercial support. Release $20,000 initially and the remaining $30,000 only after the week 4 readiness review.

The investment buys a tested seller workflow, reviewed evaluation coverage, measured customer actions and research-time savings, and evidence of willingness to pay and fully loaded delivery costs. Confirm staffing costs before kickoff and reduce scope if they exceed the cap.

Defer buyer planning, broad CRM integration, and cross-workflow learning experiments until the pilot earns further investment. The existing committed engineering work displaced by this allocation has not been identified; leadership must name and accept that trade-off before kickoff. Budget and staffing are illustrative classroom assumptions.

## M1 Baseline vs. Now
*Your 3-sentence AI strategy from Module 1 vs. what you'd say now:*

**M1 baseline:**

We are building an AI-powered advertising intelligence platform for media buyers and sellers. It will analyze market trends, predict opportunities, and recommend actions. The goal is to help customers make smarter advertising decisions.

**Now:**

We are betting that local TV sellers will act on evidence-backed prospecting recommendations built from AdQuest's proprietary advertising intelligence, and we will validate that workflow before expanding to buyers. Our proposed hybrid pricing combines a $100 monthly subscription with $10 per completed premium strategy plan, supported by measured delivery costs, explicit reliability targets, permission controls, and human approval for consequential actions. We will expand only when the pilot demonstrates customer action, time savings, paid adoption, and sustainable margins, while building defensibility through trusted data, embedded workflows, and verified improvements rather than assuming the AI itself is a moat.
