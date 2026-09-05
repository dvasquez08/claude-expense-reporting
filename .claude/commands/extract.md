---
description: Read all receipts in receipts/inbox, extract to expenses.csv, and file them
allowed-tools: Read, Write, Edit, Bash
---

Process every receipt currently in `receipts/inbox/`.

Follow the workflow, schema, categories, and rules in CLAUDE.md exactly.

1. List the files in receipts/inbox/.
2. Read each one and extract the fields.
3. Append rows to expenses.csv (create it with the header row if missing).
4. Move each file to receipts/processed/.
5. Give me the summary.

Process the whole batch without asking for confirmation on each file, then show
me the summary and every row where needs_review = yes.
