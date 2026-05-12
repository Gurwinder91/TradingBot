Log a new trade into the Nifty_Trading_Journal.xlsx file.

## Step 1 — Collect trade details

If `$ARGUMENTS` are provided, parse them. Otherwise ask the user for each field below. Confirm all values before writing.

| Field | Options / Format | Required |
|---|---|---|
| Date | DD-Mon-YY (e.g. 11-May-26) | Yes |
| Day | Monday … Friday | Yes |
| Time Entry | HH:MM (e.g. 09:30) | Yes |
| Expiry | DD-Mon-YY (e.g. 14-May-26) | Yes |
| Trade Type | CE or PE | Yes |
| Strike | Number (e.g. 24000) | Yes |
| Entry Price ₹ | Decimal (e.g. 150.50) | Yes |
| Exit Price ₹ | Decimal — leave blank if trade is still open | No |
| Stop Loss ₹ | Decimal | Yes |
| Target 1 ₹ | Decimal | Yes |
| Target 2 ₹ | Decimal | No |
| Lots | Integer | Yes |
| Result | WIN / LOSS / BREAKEVEN / OPEN | Yes |
| Filters Followed | Yes / No / Partial | Yes |
| Market Bias | Bullish / Bearish / Sideways | Yes |
| Notes / Lessons | Free text (or leave blank) | No |

## Step 2 — Write to journal

Once confirmed, build and run this Python script via Bash, substituting the actual collected values for every placeholder. Numeric fields must be bare Python literals (no quotes). Blank optional fields use `None`.

```python
import openpyxl, sys

JOURNAL = "/Volumes/coding/Trading/Trading Bot/Nifty_Trading_Journal.xlsx"

# Fill in actual values below — no placeholders
date_val    = "11-May-26"       # string
day_val     = "Monday"          # string
time_val    = "09:30"           # string
expiry_val  = "14-May-26"       # string
type_val    = "CE"              # string
strike_val  = 24000             # number
entry_val   = 150.50            # number
exit_val    = 200.00            # number or None if open
sl_val      = 120.00            # number
t1_val      = 190.00            # number
t2_val      = 220.00            # number or None
lots_val    = 2                 # integer
result_val  = "WIN"             # string
filters_val = "Yes"             # string
bias_val    = "Bullish"         # string
notes_val   = ""                # string (empty string ok)

wb = openpyxl.load_workbook(JOURNAL)
ws = wb["Trade Journal"]

# Find first empty row starting at row 5 (data starts there)
target_row = None
for r in range(5, ws.max_row + 2):
    if ws.cell(r, 1).value is None:
        target_row = r
        break

if target_row is None:
    print("ERROR: No empty rows found.")
    sys.exit(1)

# Write data columns (skip 13=P&L formula, 15=R:R formula — pre-filled)
writes = [
    (1, date_val), (2, day_val), (3, time_val), (4, expiry_val),
    (5, type_val), (6, strike_val), (7, entry_val), (8, exit_val),
    (9, sl_val), (10, t1_val), (11, t2_val), (12, lots_val),
    (14, result_val), (16, filters_val), (17, bias_val), (18, notes_val or None),
]
for col, val in writes:
    ws.cell(target_row, col).value = val

# Add formulas if this row is beyond the pre-filled range (row 55+)
if target_row > 54:
    r = target_row
    ws.cell(r, 13).value = f"=(H{r}-G{r})*L{r}*25"
    ws.cell(r, 15).value = f'=IFERROR((H{r}-G{r})/(G{r}-I{r}),"—")'

wb.save(JOURNAL)

pnl = None
if exit_val is not None and entry_val is not None:
    pnl = (exit_val - entry_val) * lots_val * 25

print(f"Logged: row {target_row} | {date_val} | {type_val} {strike_val} | {result_val}" +
      (f" | P&L ₹{pnl:,.0f}" if pnl is not None else " | Trade open"))
```

## Step 3 — Report back

Show the user the output line from the script (row number, date, strike, result, P&L). If the script errors, display the error and ask the user to correct any wrong values.
