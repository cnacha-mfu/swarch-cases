# Case Study 5: Ride-sharing Platform — "ZipRide"

## Background

ZipRide is a ride-sharing company operating in two major cities. Passengers request rides through a mobile app and are matched with nearby independent drivers. The company competes on speed of matching and reliability of pricing.

## The Organisation

- **Passengers** request rides, track drivers, and pay through the app
- **Drivers** (independent contractors) receive ride requests and navigate to destinations
- **ZipRide operations** monitors ongoing trips, handles incidents, and manages driver onboarding
- **Finance team** handles driver payouts and passenger refunds

## Current Situation

ZipRide completes around 15,000 trips per day across both cities. During morning and evening rush hours and on Friday and Saturday nights, demand exceeds driver supply and the matching algorithm struggles. The company plans to launch in 5 more cities within 18 months.

**Known problems:**
- Ride matching takes too long during peak hours, causing passengers to cancel
- Surge pricing is applied inconsistently and passengers complain it is unpredictable
- Drivers sometimes receive ride requests they are too far away to reasonably accept
- Passengers have no way to report safety concerns during a trip
- Trip history and receipts are sometimes missing after a completed ride

## What the System Needs to Do

The new system must allow:

1. Passengers to request a ride and be matched with the nearest available driver within seconds
2. Passengers to see estimated arrival time, fare, and driver details before confirming
3. Passengers to track the driver's location in real time during pickup and the trip
4. Drivers to accept or decline ride requests and navigate using in-app directions
5. Automatic fare calculation and payment processing at trip completion
6. Passengers and drivers to rate each other after every trip

## Your Task

Design a software architecture for ZipRide that addresses the problems above.

Your design should consider:
- How to match passengers and drivers quickly as both are constantly moving
- How to handle many simultaneous ride requests across a city without delay
- How to keep location data private and only visible to the matched passenger and driver
- How the system scales when launching in new cities with little notice
