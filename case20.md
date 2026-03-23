# Case Study 20: Smart Parking Management System — "ParkSmart"

## Background

ParkSmart is a city-wide smart parking system deployed across 120 car parks and 4,000 on-street parking bays in a major city. Sensors detect whether each space is occupied. Drivers can use a mobile app to find available parking, navigate to a space, and pay for their stay digitally. The city aims to reduce the time drivers spend searching for parking.

## The Organisation

- **Drivers** use the app to find, navigate to, and pay for parking spaces
- **Parking wardens** use a warden app to verify vehicles have paid
- **Car park operators** (private and city-owned) view occupancy and revenue for their sites
- **City transport authority** monitors city-wide parking usage and sets pricing policy
- **Maintenance team** receives alerts when sensors malfunction

## Current Situation

Currently, most car parks use manual ticketing machines and paper permits. On-street parking has no enforcement technology — wardens patrol on foot and manually check windscreen tickets. The city loses significant revenue to unpaid parking. Drivers report wasting 15–20 minutes searching for spaces.

**Known problems:**
- Drivers have no way to know if a car park or street area has available spaces before arriving
- Payment machines frequently break, forcing drivers to leave without paying
- Wardens cannot efficiently check whether a vehicle has paid — they rely on physical tickets
- Sensor data from different car parks arrives in different formats and frequencies
- There is no historical data on occupancy trends to inform pricing or infrastructure planning

## What the System Needs to Do

The new system must allow:

1. Sensors to report space occupancy status (free or occupied) in real time
2. Drivers to see available spaces nearby on a map and navigate to them
3. Drivers to start and stop a parking session and pay through the app
4. Wardens to check whether any vehicle is covered by a valid parking session using a licence plate lookup
5. Car park operators to view live occupancy and revenue dashboards
6. The city to apply dynamic pricing (higher rates when occupancy is high)

## Your Task

Design a software architecture for ParkSmart that addresses the problems above.

Your design should consider:
- How to collect and process real-time occupancy data from thousands of sensors reliably
- What happens when a sensor fails or goes offline — should the space be shown as available or unavailable?
- How to handle intermittent connectivity from sensors in underground car parks
- How to protect driver location and payment data collected through the app
