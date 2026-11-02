# Data Flywheel Map

> Score each loop 1-5. Your weakest loop is where competitors attack first.
> The four loops below are the M2 starting point - adapt if your product has 2 or 6 loops instead of 4.

**Product:** AdImpact SaaS Platform (including Ask AdImpact)  
**Role:** Product Manager  
**Scoring principle:** Rate what operates today, not planned capabilities. Human-reviewed backlog improvements are not automatic model learning.

## Flywheel Loops

| Loop | What It Measures | Score 1 | Score 5 | Score |
|------|------------------|---------|---------|-------|
| **Correction** | Do users fix AI outputs? Is that signal captured and reused? | No capture | Automated retraining | **2/5** |
| **Preference** | Does the product learn individual / team preferences over time? | Stateless | Deep personalization | **2/5** |
| **Domain Context** | Does usage in one area improve quality in adjacent areas? | Siloed | Cross-domain transfer | **4/5** |
| **Network** | Does each new user / team make the product better for everyone? | Isolated | Strong network effects | **1/5** |

### Correction Loop - 2/5
**What you capture today:** Ask AdImpact collects thumbs-up/down on each response and requests written feedback following a thumbs-down. Feedback becomes tickets in the product backlog. User activity is tracked and included in a daily summary email.

**How it compounds:** Feedback can lead to manual bug fixes and product improvements when the team reviews and acts on tickets. There is **no automatic learning or retraining** from user corrections today, and no confirmed process that systematically turns corrections into reusable model evaluations.

### Preference Loop - 2/5
**What you capture today:** Users save custom reports, dashboards/tile layouts, filters and subscriptions. The platform tracks activity, but persistent Ask AdImpact-specific preferences or personalization have not been confirmed.

**How it compounds:** Saved configurations make recurring user workflows easier and can increase product stickiness. They do **not** currently demonstrate that Ask AdImpact learns user or team preferences and produces increasingly personalized answers.

### Domain Context Loop - 4/5
**What you capture today:** Proprietary advertising occurrence and creative data, estimated spend, advertiser classifications, market and programming metadata, and political advertising context, collected and modeled through specialized data operations.

**How it compounds:** Continued collection and enrichment expand historical coverage and the contextual intelligence available across analyses and use cases. This is a strong proprietary domain-data advantage, though **cross-domain improvements caused by user interactions** have not been demonstrated; the score is therefore more generous than a strict usage-driven flywheel interpretation.

### Network Loop - 1/5
**What you capture today:** Product usage/activity tracking, daily usage summaries, aggregate feedback and collaboration features such as shared reports or layouts.

**How it compounds:** These signals may inform human product prioritization and broad improvements. No confirmed mechanism makes Ask AdImpact's outputs better for every customer as each additional user or team interacts with it. Collaboration is not, by itself, a network learning effect.

**Total Flywheel Score: 9/20**  
**Weakest Loop:** Network (1/5); Correction and Preference also lack automated learning.  
**Fix for weakest loop:** First make existing feedback reusable: standardize negative-feedback reasons, preserve question/answer/data context, review and label corrections, and build a regression-evaluation set. Once privacy and quality safeguards are in place, test whether validated, de-identified corrections can improve retrieval and answers across customers. Measure cross-customer quality improvements before claiming a network effect.

---

## Encroachment Threat Assessment

*Time horizons and value-at-risk percentages are illustrative breakout scenarios, not measured forecasts. “Value at risk” means customer-facing product value that could be displaced, not necessarily revenue.*

### 1. Platform Encroachment
**Attacker:** Google (Gemini) + MediaRadar (hypothetical data partnership; not an announced relationship).  
**Vector:** Put MediaRadar-like competitive advertising intelligence inside an AI assistant integrated with existing advertising, productivity and sales workflows. Own the decision-making interface while licensing rather than recreating the data.  
**Time-to-threat:** 12–24 months for meaningful displacement; a narrow pilot could be quicker.  
**% of value at risk:** 30–50% (scenario estimate).

### 2. Vertical Competitor
**Attacker:** MediaRadar.  
**Vector:** Use an established advertising intelligence dataset to match AdImpact's competitive research while offering AI-powered reporting, opportunity identification and recommendations.  
**Time-to-threat:** 0–12 months.  
**% of value at risk:** 40–60% (scenario estimate).

### 3. Adjacent Expansion
**Attacker:** Nielsen.  
**Vector:** Expand audience measurement and media-planning workflows into AI-assisted competitive advertiser intelligence and buying/selling recommendations.  
**Time-to-threat:** 12–36 months.  
**% of value at risk:** 20–40% (scenario estimate).

---

## 90-Day Encroachment Plan

*Your partner played the Big Tech attacker. What was their plan to kill you? The following is a plausible hypothetical attack scenario, not a description of actual Google or MediaRadar plans.*

**Attacker:** Google + MediaRadar (hypothetical partnership).  
**Attack vector (target the weakest loop):** Exploit AdImpact's weak Network Loop and limited preference learning. Combine comparable third-party intelligence with persistent account/territory context and integrations so user activity produces a better, more embedded workflow.  
**Weeks 1-4 - what they ship:** Pilot a Gemini-powered TV advertising intelligence assistant with licensed competitive ad data, natural-language competitor analysis, saved advertiser/market priorities and draft prospecting recommendations.  
**Weeks 5-8 - how they poach users:** Target local TV sales organizations with pilots, introductory pricing, easy import of advertiser lists and CRM/email integrations; demonstrate faster research-to-pitch workflows than navigating standalone analytics dashboards.  
**Weeks 9-12 - why users don't come back:** The assistant retains account preferences and connects intelligence to sales activity, making it costly to rebuild lists, context and workflows elsewhere. This is the attacker's intended outcome, not a guaranteed result within 90 days.  
**Your defense:** Lead with differentiated data quality, historical depth and domain-specific accuracy. In the first month, build a validated evaluation dataset from existing Ask AdImpact feedback; in the second, pilot persistent user/account preferences; in the third, test proactive opportunity recommendations integrated into existing reporting and sales workflows. Maintain control of proprietary data and measure whether answers and customer outcomes actually improve with usage.
