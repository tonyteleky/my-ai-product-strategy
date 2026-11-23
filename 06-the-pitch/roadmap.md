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

AdQuest will turn proprietary advertising intelligence into evidence-backed next actions, starting with seller prospecting and expanding into a broader AI Strategy Agent only when customer value, reliability, and economics are demonstrated.

**The case:**

1. **Why now:** Customers still spend time translating advertising data into prospect lists, competitive insights, and plans. AdQuest already has specialized advertising data and established reporting workflows. A focused AI workflow can test whether we can shorten the distance between research and action, beginning with local TV sellers rather than launching across every customer segment at once.

2. **What's defensible:** Our advantage is proprietary advertising collection, historical coverage, classification, estimation methodology, and domain context. The model and interface are copyable. We will strengthen defensibility through embedded workflows, explicit account preferences, and verified corrections that measurably improve future answers. Our current flywheel score is 9/20; automatic learning and network effects remain opportunities to validate, not established advantages.

3. **The economics:** Proposed pricing is a $100/user/month subscription plus $10 per completed premium AI Strategy Plan. For a user purchasing five plans monthly, the classroom model produces $150 revenue, $28.40 modeled COGS, and 81.1% gross margin before unestimated incremental infrastructure and review costs. At 20% premium adoption, the comparable blended modeled margin is approximately 74.5%. We will validate paid adoption and fully loaded costs; model cascading, caching, and premium usage metering help manage inference exposure.

**The risks:**

1. **Trust / failure modes:** The agent could confuse historical spending with confirmed buying intent, invent inventory availability, or present a forecast as guaranteed performance. Recommendations must distinguish observed facts, AI inferences, and verified business conditions, with sources and dates. Proposed release targets include ≥92% evaluation pass rate, 100% critical hard-check compliance, and <1% unsupported-material-claim rate. Critical failures immediately disable the affected capability.

2. **Scale / governance:** Human-review demand and infrastructure costs could grow faster than revenue. We will track review minutes, latency, cost per completed plan, and quality by workflow. Permission checks precede retrieval, confidential customer data remain isolated, and saving, sharing, exporting, or changing connected systems requires human approval. The agent cannot autonomously purchase ads, commit budgets, or guarantee outcomes.

3. **Competitive:** MediaRadar or a platform partnering with an advertising-data provider could offer similar AI recommendations. We will compete through trusted domain data and measurable workflow value, while verifying provider portability. If customers do not act on our recommendations, proprietary data alone will not justify continued expansion.

**The ask:**

Approve a capped **$50,000, 12-week validation pilot** for up to 20 local TV sellers, supported by one dedicated engineer and fractional Product, data/analyst, security, and commercial support.

This is an illustrative planning budget; confirm fully loaded staffing and operating costs before kickoff and reduce scope if necessary.

Release up to **$20,000 for the first four weeks**, then the remaining **$30,000** only after the workflow, evaluation coverage, permissions, and operational ownership pass readiness review.

Stop expansion if the pilot misses either the **30% recommendation action rate** or **20% research-time reduction** target by week 8. At week 12, revise or stop the proposed paid rollout if conversion is below **20%** or fully loaded cohort gross margin is below **65%**. H2 and H3 expansion require separate approval.

## M1 Baseline vs. Now
*Your 3-sentence AI strategy from Module 1 vs. what you'd say now:*

**M1 baseline:**

We are building an AI-powered advertising intelligence platform for media buyers and sellers. It will analyze market trends, predict opportunities, and recommend actions. The goal is to help customers make smarter advertising decisions.

**Now:**

We are betting that local TV sellers will act on evidence-backed prospecting recommendations built from AdQuest's proprietary advertising intelligence, and we will validate that workflow before expanding to buyers. Our proposed hybrid pricing combines a $100 monthly subscription with $10 per completed premium strategy plan, supported by measured delivery costs, explicit reliability targets, permission controls, and human approval for consequential actions. We will expand only when the pilot demonstrates customer action, time savings, paid adoption, and sustainable margins, while building defensibility through trusted data, embedded workflows, and verified improvements rather than assuming the AI itself is a moat.
