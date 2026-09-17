# Work Pack Schema

Use this schema for request intake and as the underlying record for weekly briefs, analysis, drafts, and handoffs. Omit fields that are genuinely irrelevant; never omit a known risk, dependency, source, or approval requirement.

## Core record

| Field | Required content |
| --- | --- |
| Client / brand | Named entity from the source; preserve ambiguity if unresolved |
| Campaign / market | Campaign, product, channel, or market in scope |
| Source request | Faithful summary of what was asked, without interpretation disguised as fact |
| Source evidence | Message/file/calendar reference, subject/title, timestamp, and link or locator when available |
| Requested outcome | The business or operational result being sought |
| Deliverable | Weekly report, MTD update, performance overview, setup recommendation, demo, content proposal, draft, etc. |
| Owner | Confirmed person/team, or `Unassigned` |
| Deadline | Absolute date/time and timezone, or `Not stated` |
| Priority | P0–P3 plus the reason under the decision rules |
| Status | Ready / In progress / Blocked / At risk / Needs approval / Done |
| Dependencies | Inputs, access, preceding work, or decisions required |
| Missing data | Only information that can change the result or confidence |
| Facts | Source-supported observations |
| Inferences | Interpretation, evidence, confidence, and alternative explanation when material |
| Decision needed | Choice, decision owner, deadline, and consequence of delay |
| Recommendation | Action, rationale, expected effect, downside, confidence, approval boundary |
| Next action | Concrete verb-led step, owner, and deadline |
| Draft / artifact | Prepared reply, analysis, spreadsheet brief, demo brief, or content recommendation |

## Concise weekly brief

Order the brief by consequence rather than source:

1. **Top priorities:** up to five items that materially affect delivery, performance, risk, or decisions.
2. **Decisions needed:** choice, owner, deadline, evidence, and consequence of delay.
3. **Execution status:** weekly reporting, MTD pacing, campaign/ad setup, demos, content optimization.
4. **Performance exceptions:** material variance, likely cause, confidence, and next check.
5. **Follow-ups:** owner and absolute deadline.
6. **Data gaps:** only gaps that limit a decision or deliverable.
7. **Questions:** at most three high-impact questions.

## Performance analysis fields

For every metric comparison, record:

- metric definition and unit;
- source/platform and extraction time;
- date range and timezone;
- actual, plan/baseline, absolute variance, and percentage variance when calculable;
- attribution window, currency, tax/fee treatment, and conversion definition when relevant;
- known data latency or completeness issue;
- whether the variance crosses an approved threshold;
- interpretation and confidence.

Do not compare values that use different definitions as if they were equivalent. If reconciliation is impossible, present a mismatch log and the decision needed on source authority.

