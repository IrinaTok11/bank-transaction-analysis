# Data

## Source file

`merged_statements_.xlsx` — bank statements from multiple sources merged via SQL into a single flat table.

## Schema

| Column | Type | Description |
|---|---|---|
| `Date` | Date | Transaction date |
| `Bank` | Text | Bank code |
| `Counterparty` | Text | Counterparty name |
| `Amount` | Decimal | Transaction amount |
| `Direction` | Text | `IN` or `OUT` |
| `IsSuspicious` | 0/1 | Suspicious activity flag |
| `IsRoundNumber` | 0/1 | Round-number structuring flag |
| `IsNewCounterparty` | 0/1 | First appearance of counterparty |
| `MonthNum` | Integer | Month number (1–12) |

## Flexibility

The dashboard reads whatever is in `merged_statements_.xlsx` — number of banks, accounts, and date range are derived dynamically from the data. Replace the file with any merged statement export and refresh.

## Privacy

File contains anonymised / sample data. Do not commit raw statements with real identifiers.
