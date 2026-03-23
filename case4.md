# Case Study 4: Online Banking System — "NeoBank"

## Background

NeoBank is a fully digital bank with no physical branches. Customers open accounts, transfer money, pay bills, and manage finances entirely through a mobile app and web portal. The bank is licensed and regulated, meaning it must comply with strict financial and data protection laws.

## The Organisation

- **Customers** manage accounts, make transfers, and pay bills
- **Customer support agents** handle disputes, account issues, and fraud reports
- **Compliance team** monitors transactions for suspicious activity
- **Bank management** tracks financial performance and regulatory reporting

## Current Situation

NeoBank has 150,000 active customers and processes around 500,000 transactions per day. The bank has grown rapidly through referrals but the original system was not built to handle this volume. Regulators have flagged concerns about the bank's fraud detection capabilities.

**Known problems:**
- Transaction processing occasionally takes several minutes instead of seconds
- The system has experienced two outages in the past six months, each lasting over an hour
- Fraud detection is mostly manual — the compliance team reviews flagged transactions the next day
- Customers cannot see a full history of their transactions beyond 3 months
- There is no multi-factor authentication, which is now required by regulation

## What the System Needs to Do

The new system must allow:

1. Customers to view account balances and full transaction history
2. Customers to transfer money between accounts (internal and external banks)
3. Customers to pay bills and set up recurring payments
4. The system to detect and flag suspicious transactions in real time
5. Customer support agents to view account activity and initiate dispute resolutions
6. Compliance team to generate regulatory reports on demand

## Your Task

Design a software architecture for NeoBank that addresses the problems above.

Your design should consider:
- How to ensure every transaction is accurate and never lost, even if the system partially fails
- How to keep the system available at all times, including during maintenance
- How to protect customer accounts from unauthorised access and fraud
- What level of audit logging is needed and how long records must be kept
