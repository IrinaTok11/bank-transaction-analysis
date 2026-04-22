# DAX measures

All measures live in the `Sheet1` table and are versioned here as a single file.

## Groups

| Group | Measures |
|---|---|
| Core aggregates | `Total Transactions`, `Total Inflow`, `Total Outflow`, `Total Turnover`, `Net Cash Flow`, `Bank Count` |
| Suspicious activity | `Suspicious Count`, `Suspicious %`, `Suspicious Amount CP`, `Flagged Counterparties`, `Round Number Count` |
| Counterparty | `CounterpartyRisk`, `CounterpartyColor`, `CP Period`, `CP Start Month`, `CP End Month` |
| Labels | `Avg per Month Label`, `Inflow % Label`, `Outflow % Label`, `Suspicious Pct Label`, `Top Risk Bank` |

## DAX style conventions

- Comma-separated arguments.
- `VAR / RETURN` pattern for multi-step calculations.
- `DIVIDE(numerator, denominator, 0)` — safe division with 0 as fallback.
- `FORMAT(..., "en-GB")` — locale-explicit date formatting.
