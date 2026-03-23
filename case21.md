# Case Study 21: Digital Wallet & Peer-to-Peer Payment System — "PayMate"

## Background

PayMate is a mobile digital wallet that allows users to store money, send and receive payments from other users, pay merchants, and top up their balance from a bank account. It targets underbanked users who may not have a traditional bank account. The platform operates in four countries, each with its own currency and financial regulations.

## The Organisation

- **Users** top up their wallet, send money, receive money, and pay merchants
- **Merchants** (small businesses) accept PayMate payments through a QR code or payment link
- **PayMate compliance team** monitors for money laundering and fraud
- **Finance team** manages float accounts, currency exchange, and regulatory reporting
- **Customer support** handles disputed transactions and account access issues

## Current Situation

PayMate has 3 million active users and processes around 400,000 transactions per day. The platform must operate in near-real time — users expect money to appear in the recipient's wallet instantly. Regulatory requirements vary per country, including different identity verification standards and transaction limits.

**Known problems:**
- Transactions occasionally fail halfway, leaving one user debited but the other not credited
- Users in some countries are not completing the identity verification step, which creates regulatory risk
- Fraudulent accounts are used to move money between wallets quickly before being detected
- Customer support has no way to temporarily freeze a suspicious account without taking it fully offline
- There is no way for users to dispute a payment they believe was made in error

## What the System Needs to Do

The new system must allow:

1. Users to top up their wallet from a linked bank account or cash agent
2. Users to send money to another PayMate user instantly using a phone number or QR code
3. Merchants to generate payment requests and receive funds in their merchant wallet
4. Users to view their full transaction history
5. Compliance team to flag, freeze, or investigate suspicious accounts
6. The system to enforce transaction limits and identity verification rules per country

## Your Task

Design a software architecture for PayMate that addresses the problems above.

Your design should consider:
- How to ensure that a transfer between two wallets either fully completes or fully reverses — never a partial state
- How to detect suspicious transaction patterns quickly enough to act before funds are moved
- How to apply different regulatory rules per country without duplicating the entire system
- How to scale to handle sudden spikes in transactions (e.g., public holidays, salary day)
