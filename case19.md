# Case Study 19: Event Ticketing System — "TicketRush"

## Background

TicketRush is an online platform that sells tickets for concerts, sports events, theatre shows, and festivals. Event organisers list their events and set up seating plans, and customers purchase tickets which are delivered digitally. The platform also handles resale between customers.

## The Organisation

- **Event organisers** create events, configure seating or standing sections, and set pricing
- **Customers** browse events, select seats, purchase tickets, and present them at entry
- **Venue staff** scan tickets at gates to validate entry
- **TicketRush finance** collects platform fees and pays organisers after events
- **Customer support** handles refund requests and invalid ticket disputes

## Current Situation

TicketRush sells tickets for around 200 events per month. The challenge is that ticket sales for major events — especially popular musicians or championship sports games — result in enormous simultaneous demand. Thousands of customers attempt to buy tickets the moment sales open.

**Known problems:**
- When a popular event goes on sale, the website crashes due to the sudden surge in traffic
- Customers frequently reach checkout only to find their selected seats were taken while they were filling in payment details
- Duplicate tickets are occasionally issued, causing entry disputes at the venue
- Scalpers use automated bots to buy large quantities of tickets immediately, then resell at inflated prices
- Customers who buy resale tickets sometimes receive fraudulent tickets that fail at the gate

## What the System Needs to Do

The new system must allow:

1. Event organisers to create events with seat maps and pricing tiers
2. Customers to browse events and select available seats
3. Seats to be temporarily held while a customer completes checkout
4. Secure payment processing and digital ticket delivery
5. Venue staff to scan and validate tickets at entry using a mobile app
6. Customers to resell tickets through the platform with anti-fraud verification

## Your Task

Design a software architecture for TicketRush that addresses the problems above.

Your design should consider:
- How to handle thousands of simultaneous users competing for a limited number of seats at the moment sales open
- How to prevent the same seat from being sold to two customers
- How to detect and limit bot-driven bulk purchasing
- How to ensure that a ticket cannot be copied or forged and that each one is only valid once
