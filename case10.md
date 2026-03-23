# Case Study 10: Airline Reservation System — "SkyBook"

## Background

SkyBook is the reservation system for a regional airline operating 40 routes across 15 cities. The airline sells tickets through its own website, a mobile app, and third-party travel agencies. It handles check-in, seat selection, baggage, and boarding processes digitally.

## The Organisation

- **Passengers** search flights, book tickets, select seats, and check in online
- **Travel agents** book on behalf of customers through an API integration
- **Ground staff** manage check-in desks, boarding gates, and baggage
- **Flight operations** monitors schedules, delays, and aircraft assignments
- **Revenue management** adjusts ticket pricing dynamically based on demand

## Current Situation

The airline handles around 200 flights per day carrying up to 25,000 passengers. Ticket sales happen continuously, but the heaviest booking periods are weekends and school holidays. The current system was built in the 1990s and has not been significantly updated.

**Known problems:**
- Overbooking occurs occasionally when ticket counts are not synchronised correctly across sales channels
- Online check-in opens 24 hours before departure but the system becomes slow as all passengers check in near departure time
- When a flight is delayed or cancelled, passengers are not notified automatically
- Seat selection is only possible for some fare types but this rule is inconsistently enforced
- Travel agency bookings sometimes take up to 10 minutes to be confirmed

## What the System Needs to Do

The new system must allow:

1. Passengers to search flights by route and date, and view available seats and fares
2. Passengers to book tickets, select seats, and add baggage options
3. Online check-in within 24 hours of departure
4. Ground staff to access passenger manifests and manage boarding
5. Automatic notification to passengers when a flight is delayed or cancelled
6. Revenue management to update pricing rules without system downtime

## Your Task

Design a software architecture for SkyBook that addresses the problems above.

Your design should consider:
- How to prevent two passengers from booking the same seat simultaneously
- How to keep inventory consistent across the airline's own channels and third-party agents
- What should happen if a flight is cancelled — how are all affected passengers notified and re-booked?
- How to ensure the system remains operational during the busy departure window when load is highest
