---
description: Build a monthly Excel report from expenses.csv for the current month
allowed-tools: Read, Write, Bash
---

Read `expenses.csv`. Determine the current month and year, and produce an Excel
file named `expense-report-<month-name-lowercase>-<year>.xlsx`
(e.g. expense-report-march-2026.xlsx), overwriting it if it already exists.

Include ONLY rows whose `date` falls in the current calendar month. Two sheets:

1. "Expenses" — this month's rows, bold header, currency-formatted amounts, a
   bold TOTAL row, and any needs_review = yes row highlighted amber.
2. "Summary" — this month's total per category (sorted high to low), plus a
   grand total and receipt count.

Save to the project root and tell me the filename and this month's grand total.
