# Case Study 8: Hotel Booking Platform — "StayEasy"

## Background

StayEasy is an online travel platform that allows customers to search and book hotel rooms from a catalogue of 10,000 partner hotels worldwide. Hotels connect to StayEasy through an integration layer to share room availability and receive bookings. The company earns a commission on each booking.

## The Organisation

- **Customers** search for hotels, compare options, and make reservations
- **Hotel partners** manage their room inventory, pricing, and booking calendar through a partner portal
- **StayEasy operations** handles customer complaints, refund requests, and partner onboarding
- **Finance team** manages commission collection and partner payouts

## Current Situation

StayEasy processes around 3,000 bookings per day. Demand spikes dramatically during public holidays and when popular destinations run events. The platform currently lists room availability by polling each hotel's system every 30 minutes, which means availability shown to customers is often outdated.

**Known problems:**
- Customers occasionally book a room that is actually no longer available, causing the booking to fail after payment
- Hotel partners have no self-service way to update room pricing quickly — they must email StayEasy
- Search results take 8–12 seconds to load when filtering across many hotels
- Cancellation and refund rules differ per hotel but are applied incorrectly by the system
- There is no way for customers to see reviews or ratings for hotels listed on the platform

## What the System Needs to Do

The new system must allow:

1. Customers to search hotels by location, dates, price, and star rating
2. Customers to book and pay for a room, with instant confirmation
3. Hotel partners to update room availability, pricing, and policies through a self-service portal
4. The system to reflect room availability changes in real time or near-real time
5. Customers to leave reviews and ratings after their stay
6. Operations staff to process cancellations and refunds according to each hotel's policy

## Your Task

Design a software architecture for StayEasy that addresses the problems above.

Your design should consider:
- How to prevent double-booking when multiple customers attempt to book the last available room simultaneously
- How to keep search fast when querying across thousands of hotels and date combinations
- How to integrate with hotel partners who each have different systems and data formats
- How to handle failed payments gracefully without leaving a booking in an inconsistent state
