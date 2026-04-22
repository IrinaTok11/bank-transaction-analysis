# Deneb visuals

Vega-Lite specs for all four custom Deneb visuals in the report.  
Clean JSON — no `//` or `/* */` comments. Specs are versioned here for reproducibility.

## Files

| File | Visual | Description |
|---|---|---|
| `in_out_split.json` | In / Out Split | Normalised stacked bar showing inflow vs outflow ratio |
| `risk_by_account.json` | Risk by Account | Ranked horizontal bars with avg risk reference line per bank account |
| `suspicious_activity_timeline.json` | Suspicious Activity Timeline | Gantt-style bars showing activity window per flagged counterparty |
| `top_counterparties.json` | Top Counterparties | Horizontal bar chart ranked by volume; suspicious counterparties highlighted in red |

## How to re-use a spec

1. In Power BI Desktop, add a **Deneb** visual to the canvas.
2. Open the Deneb editor → **New specification** → paste the JSON.
3. Map the required fields from `Sheet1` (see field references in each spec).

## Field references

| Spec | Fields used |
|---|---|
| `in_out_split` | `Total Inflow`, `Total Outflow` |
| `risk_by_account` | `Bank`, `Suspicious Count`, `Total Transactions` |
| `suspicious_activity_timeline` | `Counterparty`, `Suspicious Amount CP`, `Suspicious Count`, `CP Start Month`, `CP End Month`, `CP Period` |
| `top_counterparties` | `Counterparty`, `Total Turnover Line`, `IsSuspicious` |
