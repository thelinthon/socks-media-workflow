# Pacing and Forecast

Use this reference for MTD execution, weekly delivery status, spend pacing, and completion forecasts.

## Inputs

Require campaign budget, actual spend through a confirmed cutoff, active start/end dates, currency, and any planned pauses or non-linear daily allocation. Prefer the approved daily budget curve when available.

If only dates are available, use linear elapsed-time pacing as an explicitly labeled estimate:

- elapsed fraction = active elapsed days / total active days;
- spend fraction = actual spend / approved budget;
- pacing gap = spend fraction - elapsed fraction;
- pacing index = spend fraction / elapsed fraction;
- linear forecast = actual spend / elapsed fraction.

Use inclusive active days unless the approved plan defines another convention. Do not count days before launch, after completion, or during confirmed pauses.

## Classification

Use team- or client-approved thresholds. If none are supplied, report the numeric gap and write `Threshold not defined`; do not invent a universal red/amber/green rule.

Distinguish:

- **Spend pacing:** whether budget consumption matches the approved curve.
- **KPI delivery:** whether the contracted or planned output is being achieved.
- **Cost efficiency:** whether CPM/CPV/CPC/CPA meets its benchmark.
- **Completion:** whether the campaign has reached its confirmed end condition.

An underspent campaign can still exceed KPI. An efficient campaign can still overspend. Never collapse these into one label.

## Forecast caveats

Linear forecasts are unreliable when launch ramp-up, platform learning, scheduled bursts, inventory constraints, manual caps, makegoods, or approved reallocations materially change daily delivery. State the limitation and use the approved daily curve or scenario range when available.

Every recommendation must identify remaining budget, remaining days, likely completion risk, downside, owner, and approval requirement. Never execute a budget, bid, targeting, or status change.
