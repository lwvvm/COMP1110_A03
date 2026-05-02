# COMP1110 A03 - PocketHK

PocketHK is a local-first personal budgeting web app for quick daily finance tracking.
It focuses on fast transaction logging, simple budget control, and clear monthly summaries.

## Project Overview

- Record income and expense transactions with categories, notes, and dates
- Manage multiple accounts and track balances in one place
- Set monthly budgets and view basic spending summaries
- Review insights with charts for categories and trends
- Local-first: data stays in your browser storage

## Key Features

- Transaction logging (income/expense), category, date, note, account
- Monthly dashboard: net flow, budget usage, net worth summary
- Accounts: add/edit balances, transfer between accounts
- Insights: category breakdown and simple trends
- Receipt OCR: optional auto-fill from receipt images
- CSV export for transaction history

## Tech Stack

- HTML + Tailwind CSS (CDN)
- Vanilla JavaScript
- Chart.js
- Tesseract.js
- Browser LocalStorage

## Use the App

Open the deployed version directly:

- https://lwvvm.github.io/COMP1110_A03/

## Data Storage

- Data is stored in LocalStorage with key: pockethk-v3-eng
- Clearing browser site data will remove saved app data

## Known Limitations

- OCR accuracy depends on receipt quality
- Data is local to one browser/device unless exported
