# COMP1110 A03 - PocketHK

PocketHK is a local-first personal budgeting web app built for quick daily finance tracking.
It supports expense/income recording, account management, monthly budgeting, visual insights, and receipt OCR-assisted form filling.

## Project Plan

- Project plan document: https://docs.google.com/document/d/13agy1rkJSFGr5e16rZ1nf5E-pS5grBgb4C_Dy_cXGEA/edit?tab=t.0

## Key Features

- Record transactions with:
	- amount, currency, type (expense/income), category, date, note, account
	- spending mood tags for expense entries
- Receipt OCR auto-entry:
	- upload a receipt image to prefill amount/date/note/category (best-effort)
- Monthly dashboard:
	- total net worth (aggregated across accounts with FX conversion to HKD)
	- monthly budget usage
	- monthly net flow
- Insights tab:
	- expense and income category breakdown charts
	- trend forecast (income vs expense)
	- spending mindset analytics
- Budget tab:
	- total monthly budget
	- category budget setup and progress tracking
- Accounts tab:
	- add cash/card/e-wallet accounts
	- edit account current balance
	- transfer between accounts
	- optional account PIN setup
- CSV export for transaction history

## Tech Stack

- HTML + Tailwind CSS (via CDN)
- Vanilla JavaScript
- Chart.js (charts)
- Tesseract.js (OCR)
- Browser LocalStorage (data persistence)

## Run the App

Use the deployed version directly:

- https://lwvvm.github.io/COMP1110_A03/



## File Structure

```text
.
|- index.html        # main application (UI + logic)
|- index_test.html   # testing/alternate page snapshot
`- README.md
```

## Data Storage

- Data is stored in LocalStorage with key: pockethk-v3-eng
- Main stored state includes:
	- selectedMonth
	- settings (monthly budget, category budgets, quick presets)
	- accounts
	- transactions
- Clearing browser site data or local storage will remove saved app data.

## Usage Guide

1. Add one or more accounts in the Accounts tab.
2. Record income/expense transactions in Overview.
3. Set monthly and category budgets in Budget.
4. Check trends and behavior in Insights.
5. Export CSV if needed for reporting or backup.

## Known Limitations

- OCR extraction quality depends heavily on image quality and receipt format.
- All data is local to one browser/device unless exported manually.
- Currency conversion uses fixed rates defined in source code.

## Demo Checklist

For a clean demonstration, prepare these before presenting:

- at least 2 accounts with different account types
- at least 10-15 transactions across multiple categories
- both income and expense records in the selected month
- one transfer between accounts
- monthly budget plus 2-3 category budgets
- one OCR scan example (optional)

## Authors

- COMP1110 A03 team
