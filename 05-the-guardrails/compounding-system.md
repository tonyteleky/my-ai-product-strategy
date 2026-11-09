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

*Working proposal for class discussion; implementation and control effectiveness remain to be verified.*

## Agent Topology
<!-- If using agents: what can each agent do? What can't it do? Who approves what? -->

## Shadow AI Audit

| Tool | Owner | Risk Level | Decision |
|------|-------|-----------|----------|
| | | H / M / L | keep / govern / kill |
| | | H / M / L | keep / govern / kill |
| | | H / M / L | keep / govern / kill |

**Total tools found:**
**Tools after triage:**
**Estimated hidden spend:**
