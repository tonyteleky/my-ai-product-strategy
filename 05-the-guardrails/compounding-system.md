# Compounding System Design — AdQuest

## Feedback Loops

| Loop | Input | Output | Compounds? | Status |
|------|-------|--------|-----------|--------|
| Recursive learning | User-reported errors, verified corrections, and failed answers | Expanded evaluation dataset and tested improvements to retrieval, calculations, and answers | Y, once corrections reliably improve future answers | Missing — end-to-end process not yet verified |
| Cross-domain transfer | Validated definitions, entity mappings, and analytical methods across advertising workflows | More consistent answers across related analyses without transferring confidential customer context | Y, if improvements carry across workflows | Missing — shared improvement path not yet verified |
| Network intelligence | Aggregated, privacy-reviewed patterns in question types, failures, and usefulness across customers | Better prioritization and reusable improvements to common queries | Y, if aggregate insights measurably improve answers | Missing — aggregation and privacy controls not yet verified |

**Broken loop identified by partner:**  
Pending peer review. Proposed gap to challenge: user corrections may reach support or product without becoming verified evaluation cases and released improvements. Collecting feedback alone does not establish learning.

**Fix plan:**  
Product owns weekly triage of reported errors with a designated data/engineering owner. Validate each correction, add a regression case, test the fix, and notify the reporter of the outcome. Track correction-to-fix time and repeat-error rate. Close material issues only after the fix passes evaluation.

## Context Connectivity

Proposed knowledge flow: user question → permission-checked advertising data → analysis → sourced answer → user feedback → product/data triage → evaluation case → engineering fix → validated release.

Shared definitions, entity mappings, source dates, and calculation methods should connect retrieval, analysis, support, and product. Customer-confidential queries, uploads, and analyses remain isolated by account; reusable learning must exclude confidential content.

Potential silos to investigate: support feedback disconnected from engineering, data corrections disconnected from retrieval, and policy changes disconnected from agent permissions. Each material finding needs one accountable owner and a tracked resolution.

## Governance Policy

**Scope:**  
AI-assisted search, analysis, and summaries of authorized advertising data. Enforce permissions before retrieval, isolate customer-confidential information, and block credentials and unnecessary personal data. Use approved model providers; no shared-model training on customer content without explicit authorization.

**Autonomy boundaries:**  
Auto: retrieve permitted data, calculate metrics, and draft answers with sources, reporting periods, and limitations. Human approval: save, overwrite, export, share, or change connected systems. Never auto: purchase ads, commit budgets, change campaigns, or make contractual promises. Never fabricate metrics or guarantee outcomes.

**Escalation triggers:**  
Stop the affected action when sources conflict, material claims lack evidence, requested data is unavailable, permissions fail, or restricted data appears. Route analytical issues to product/data, suspected disclosure to security, and contractual questions to legal. Suspected cross-customer exposure blocks the affected retrieval path pending security review.

**Audit cadence:**  
Weekly — Product reviews 25 sampled answers and all reported material errors. Before every release — engineering tests accuracy, calculations, permissions, and regressions; access-control failures block release. Quarterly — product, security, and legal review policy and incidents. Engineering, security, and legal owners must be named before launch.

**Regulatory exposure (EU AI Act / other):**  
Legal/security must assess applicable privacy and AI requirements, advertising-data licenses, customer agreements, and model-provider terms. EU AI Act applicability and risk tier remain unassigned pending review of intended use and markets. Document permitted data use, retention, deletion, vendor processing, and customer access controls.

## Agent Topology

Proposed boundaries if AdQuest uses agents; architecture remains to be verified.

| Agent / function | Can do | Cannot do | Who approves / owns |
|------------------|--------|-----------|---------------------|
| Retrieval | Read authorized advertising data | Expand permissions, access another customer's confidential data, or modify records | Engineering enforces access; authorized administrators approve permission changes |
| Analysis | Calculate metrics and draft sourced answers | Invent data, guarantee outcomes, or make commercial commitments | Product/data reviews disputed answers; engineering owns validation |
| Sharing / export | Prepare content for review | Save, overwrite, export, or send without explicit approval | User approves content and destination |

Tools must be allow-listed, rate-limited, and logged. Retrieved content is treated as data, not instructions. Memory defaults to the session; persistent memory requires an approved purpose and retention rule. Customer-confidential content cannot enter shared memory. Permission or validation failures stop the chain; engineering owns handoffs.

## Shadow AI Audit

User-side audit: how customers use external AI around AdQuest. Rows below are hypotheses to validate, not confirmed findings. The original template's internal-tool fields are adapted to workaround, signal, frequency, and build / partner / ignore decisions.

| Tool / potential workaround | Signal / source to investigate | Frequency | Proposed decision |
|-----------------------------|--------------------------------|-----------|-------------------|
| ChatGPT / Claude summarizes exported AdQuest data into reports | Workflow gap — reporting interviews and export-related support requests | Unknown | Build source-linked summaries if recurring demand is confirmed |
| Another AI verifies or explains an AdQuest answer | Trust gap — disputed answers and interviews about verification habits | Unknown | Build better sourcing, calculation transparency, and reliability |
| External AI combines AdQuest exports with CRM or campaign data | Capability gap — interviews about analyses users cannot complete in AdQuest | Unknown | Partner through permission-controlled integrations |
| Zapier / Make + an LLM creates recurring briefings | Workflow gap — API usage and customer-built automations | Unknown | Partner through approved automation with sharing controls |
| General AI tools turn AdQuest findings into presentations or marketing copy | Workflow gap — observe users preparing deliverables | Unknown | Ignore + monitor unless evidence establishes a core product need |

**Total tools / workarounds found:**  
None confirmed yet; five workaround hypotheses identified.

**Tools / workarounds after triage:**  
Five candidates: 2 build / 2 partner / 1 ignore + monitor. Decisions remain provisional pending frequency and strategic-fit evidence.

**Estimated hidden spend / adjacent spend:**  
Unknown. Validate external subscription costs and the portion attributable to AdQuest-related workflows; avoid double-counting subscriptions.

**Next step:**  
Conduct five customer workflow interviews and review support requests mentioning ChatGPT, Claude, exports, reporting, or automation. Record observed examples, frequency, data shared externally, and spending before committing roadmap work.

**Priority question:**  
Are users reaching for external AI to extend AdQuest's workflow or to verify answers they do not trust? Workflow gaps suggest integration or expansion; trust gaps require reliability improvements.
