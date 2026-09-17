# Report Data QC

Use this reference before interpreting any spreadsheet, dashboard export, platform report, or weekly pack.

## Source hierarchy

Do not assume the Summary sheet is authoritative. Determine the approved authority for each field:

- plan identity, objective, dates, budget, and KPI: approved flowchart or signed-off media plan;
- actual delivery and spend: approved platform export or ReportsHub extract;
- derived metrics: recompute from source numerators and denominators when possible;
- narrative: never an authority for numbers unless the user explicitly confirms it as the approved record.

When authority is not defined, show the conflict and request the decision owner. Do not average or silently choose a value.

## Required checks

For every material campaign line, verify:

1. **Identity:** client, campaign, market, platform, objective, buying type, material, landing destination, and flight distinguish the row from similar lines.
2. **Period:** reporting window, actual extraction time, campaign start/end, timezone, and data latency are compatible.
3. **Plan:** budget, planned KPI, currency, fees/tax, and revisions match the approved version.
4. **Actuals:** spend, impressions, views, clicks, and conversions trace to the correct platform block and period.
5. **Formulas:** Summary references point to the intended campaign and metric; totals do not include duplicate blocks or future periods.
6. **Metric integrity:** CPM = spend/impressions*1000, CPV = spend/views, CPC = spend/clicks, CTR = clicks/impressions, VTR = views/impressions, subject to the platform's confirmed definitions.

## Stop conditions

Mark the affected conclusion `Blocked by QC` when:

- an actual appears before the confirmed launch date;
- a formula points to another campaign, creator, landing destination, or objective;
- Summary and approved plan disagree on budget or dates;
- the same delivery is included in more than one campaign total;
- the numerator, denominator, currency, or attribution definition is unknown;
- broken formulas or stale caches affect a material result.

Do not block unaffected campaigns. Produce a mismatch log with source, cell/range or record locator, impact, proposed owner, and next check.

## QC output

Lead with client-facing risk:

| Severity | Use when | Response |
| --- | --- | --- |
| P0 | Active spend or client-facing totals may be materially wrong | Contain the output; require reconciliation before release |
| P1 | One campaign conclusion or optimization decision is unreliable | Exclude or caveat the line; assign correction |
| P2 | Formatting, non-material formula, or unused field issue | Log for repair without blocking the report |

Never repair source files unless the user asks. A corrected analytical view must remain traceable to the original values.
