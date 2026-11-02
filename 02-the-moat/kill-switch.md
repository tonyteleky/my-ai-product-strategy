# Kill Switch Audit

**Product:** AdQuest SaaS Platform — Ask AdQuest  
**Goal:** Demonstrate an AI model/provider switch, with quality checks and rollback, within 48 hours.  
**Evidence note:** Underlying architecture and provider configuration have not been verified with the third-party AI development partner. Unknown is not the same as absent; risks below are provisional.

## Vendor Dependency Assessment

| Dimension | Current State | Risk Level | 48-Hour Action |
|-----------|--------------|------------|---------------|
| **Provider** | Ask AdQuest uses third-party AI implementation support (a third-party AI development partner). The specific underlying LLM provider(s), models, terms and approved alternatives need confirmation. The third-party AI development partner is an implementation vendor, not necessarily the LLM provider. | **M** | Confirm active models/providers, API and data-handling dependencies, contractual restrictions and at least one feasible backup provider. |
| **Abstraction** | Not confirmed whether model API calls and provider-specific functionality are isolated behind an abstraction layer or embedded in application logic. | **H** | Ask engineering and the third-party AI development partner to map provider-specific calls; verify or prototype a provider-neutral interface for a limited set of core Ask AdQuest queries. |
| **Routing** | No verified ability to route across multiple LLMs or fail over automatically. | **H** | Identify a backup model, validate credentials/access and implement or test a configuration-driven manual failover path for a narrow workflow. |
| **Eval** | Thumbs-up/down, optional negative-feedback text, backlog tickets and daily activity reports exist. No automatic learning occurs. An automated, provider-neutral evaluation harness has **not** been confirmed. | **H** | Assemble representative questions and known failures, define factuality/data-grounding and latency criteria, then run a small regression test against primary and backup models. |

## Portability Score

**Partial (provisional; 48-hour readiness unproven).** AdQuest has feedback and product-management processes, but a validated provider swap is not confirmed. If technical review shows tightly coupled calls and no viable backup, reclassify as **Locked** until remediation is demonstrated.

### Actions to reach 48-hour readiness

- **This week:** Confirm provider and implementation dependencies, data boundaries, current routing, and test coverage with the third-party AI development partner and engineering.
- **This month:** Verify/build provider abstraction and establish a working secondary-model path for priority Ask AdQuest tasks.
- **This quarter:** Automate evaluations using representative questions and reviewed negative feedback; rehearse a complete failover and rollback, demonstrating quality, security, costs and operation within 48 hours.

## If [primary vendor] doubles pricing tomorrow:

**48-hour response:** Quantify cost exposure and usage by model/task; negotiate or apply spend controls and rate limits without compromising critical functionality. Activate a preapproved backup **only if** its data/security requirements and regression tests pass; otherwise temporarily constrain nonessential AI features while engineering evaluates alternatives. A safe full-provider switch cannot currently be promised in 48 hours.

## If [primary vendor] ships a competing product:

**Defensible asset:** AdQuest's proprietary advertising collection, identity/classification, historical datasets, estimation methodology, market/political domain context, and customer-specific workflows—not the commodity LLM itself. Review vendor agreements, access and data-use terms; protect data and retrieval boundaries; prioritize a model-agnostic architecture and strengthen workflow personalization. If the vendor is the third-party AI development partner rather than the underlying model provider, assess implementation/IP and operational continuity separately.
