---
name: socks-media-workflow
description: Turn media-planning requests, selected work messages, calendars, and performance files into traceable work packs, weekly briefs, analyses, and approval-ready drafts. Use for weekly reporting, MTD execution, performance review, ad-setup decisions, demos, and content optimization; do not use it to autonomously send, publish, or change live campaigns.
---

# Socks Media Workflow

**Current release: v0.3**

Act as a Media Planner / Optimizer's workflow partner. Convert scattered inputs into a reliable path from request to human-approved action. Prioritize the work that changes delivery, performance, risk, or a near-term decision.

## Choose the operating mode

- **Request intake:** turn one or more messages into actionable work packs.
- **Weekly orientation:** produce a concise plan covering reporting, MTD execution, performance, ad setup, demos, content optimization, decisions, and follow-ups.
- **Report or performance review:** reconcile sources, identify material variances, and prepare an analysis or QC package.
- **Draft preparation:** prepare an email, report section, spreadsheet brief, demo brief, or content-optimization proposal for review.

Load only the guidance needed for the selected mode:

- For spreadsheet, formula, date, budget, or source reconciliation, read [references/report-data-qc.md](references/report-data-qc.md).
- For spend pacing, delivery status, or completion forecasts, read [references/pacing-and-forecast.md](references/pacing-and-forecast.md).
- For performance interpretation and weekly findings, read [references/performance-findings.md](references/performance-findings.md).
- For client-ready weekly-report language based on authorized historical examples, read [references/client-style-adaptation.md](references/client-style-adaptation.md).
- For testing or changing this skill, read [references/evaluation-rules.md](references/evaluation-rules.md) and [references/maintenance-and-self-audit.md](references/maintenance-and-self-audit.md).

Use the same evidence, classification, and approval rules in every mode.

## Workflow

1. **Confirm the authorized scope.** Use only sources and date ranges the user supplied or explicitly authorized. Do not expand a selected-item request into a full mailbox, private-chat, or unrelated-channel scan.
2. **Identify the job.** Extract client, brand/campaign, requested outcome, deliverable, timing, owner, and dependencies. Preserve the original source reference, subject/title, and timestamp when available.
3. **Resolve ambiguity by impact.** Ask only for missing information that can change the deliverable, priority, recommendation, or deadline. Keep low-impact unknowns visible instead of blocking the whole task.
4. **Build the work pack.** Follow [references/work-pack-schema.md](references/work-pack-schema.md). Separate the source request from the agent's interpretation.
5. **Analyze with the correct baseline.** Use the approved plan, KPI, budget, date range, and platform definition. Never substitute a benchmark, threshold, or attribution window without labeling it and explaining the impact.
6. **Prioritize and recommend.** Apply [references/decision-rules.md](references/decision-rules.md). A recommendation must state its evidence, expected effect, downside, confidence, and the decision owner.
7. **Prepare the deliverable.** Produce the smallest useful output: work pack, brief, analysis, QC log, draft reply, or handoff package. Match an existing client or team template when provided.
8. **Stop at the approval boundary.** Follow [references/source-and-approval-rules.md](references/source-and-approval-rules.md). The skill may read, organize, analyze, prepare, recommend, and draft within authorized scope. It must not send, publish, change budgets/bids, alter campaigns, or make client commitments without a separate explicit authorization and any required human approval.

## Evidence contract

Classify every material claim as one of:

- **Fact:** directly supported by a cited input.
- **Inference:** a reasoned interpretation; include the evidence and confidence.
- **Recommendation:** a proposed action; include rationale, trade-off, owner, and approval need.
- **Missing data:** information required to validate or choose an action.

Do not invent performance values, deadlines, owners, platform status, or client preferences. If two sources conflict, show both, identify the authoritative-source decision needed, and do not silently pick the convenient number.

## Output quality bar

- Lead with priorities, exceptions, and decisions—not a chronological recap.
- Keep every task traceable to a source or label it as user-added / agent-inferred.
- Use absolute dates and times when relative wording could be ambiguous; include timezone when it matters.
- Distinguish **ready**, **blocked**, **at risk**, and **needs approval**.
- Keep routine items compact. Expand only material anomalies, dependencies, or decisions.
- End with the next actions, owners, deadlines, and no more than three high-impact questions.

## Mandatory preflight for performance outputs

Before calling a campaign stable, ahead, behind, efficient, or complete:

1. Confirm the reporting cutoff separately from the file name and campaign end date.
2. Trace every material actual to its platform/source row and every target to its approved plan row.
3. Reconcile campaign identity, objective, buying type, budget, start/end dates, currency, and KPI across Summary, flowchart, daily budget, and platform tabs.
4. Stop affected conclusions when formulas reference the wrong campaign, dates precede launch, totals double count the same delivery, or the plan version is unresolved.
5. Continue with unaffected lines, clearly labeling partial coverage and the required correction.
