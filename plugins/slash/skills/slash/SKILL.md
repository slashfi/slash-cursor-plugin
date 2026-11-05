---
name: slash
description: Work with a Slash business account through the Slash MCP - balances, transactions, invoices, bills, contacts, recipients and transfers. Use when the user asks about their Slash account or wants to act on it.
---

# Slash

## Before acting

- List the legal entities first when the user has more than one business, and confirm which one to use.
- Use `describe_actions` to find the right action and its inputs instead of guessing field names.

## Money movement

- Never send a transfer or pay a bill without showing the user the amount, source account, recipient and rail, and getting an explicit yes.
- Amounts are in cents. Restate them in dollars when confirming.

## Reading data

- Prefer filters (date range, status, account) over pulling everything and filtering locally.
- Transaction ids start with `agg_tx_`. Keep ids as returned.
