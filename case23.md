# Case Study 23: Fleet Management System — "TrackFleet"

## Background

TrackFleet is a logistics company operating a fleet of 600 delivery trucks across a country. Trucks carry goods from regional distribution centres to retail customers and businesses. The company competes on reliable, on-time delivery and needs to control fuel costs, maintenance expenses, and driver hours.

## The Organisation

- **Drivers** receive daily delivery schedules, update delivery status, and report issues on the road
- **Dispatchers** assign deliveries to drivers and vehicles, and reroute in response to delays
- **Fleet managers** monitor vehicle health, plan maintenance schedules, and review driver performance
- **Warehouse staff** load vehicles and confirm dispatch
- **Finance team** tracks fuel usage, overtime, and maintenance costs per vehicle

## Current Situation

Each truck is equipped with a GPS tracker and an on-board diagnostic (OBD) device that reports engine health data. Currently, GPS data is only reviewed after delivery issues occur rather than in real time. Maintenance is scheduled by calendar (e.g., every 3 months) rather than based on actual vehicle condition.

**Known problems:**
- Dispatchers have no real-time visibility of where each truck is, leading to delays when customers call to ask about their delivery
- Breakdowns are not anticipated — vehicles fail unexpectedly because maintenance is not triggered by condition data
- Drivers sometimes take unauthorised detours, increasing fuel costs
- Paper delivery receipts are lost or damaged, making it hard to prove delivery in disputes
- There is no system to alert dispatchers when a truck is behind schedule

## What the System Needs to Do

The new system must allow:

1. GPS and OBD devices on each truck to send location and engine data continuously
2. Dispatchers to see all 600 trucks on a live map with current location and delivery status
3. The system to alert dispatchers when a truck deviates from its planned route or is behind schedule
4. Fleet managers to receive maintenance alerts based on engine condition data rather than just calendar dates
5. Drivers to confirm deliveries digitally with customer signature capture on a mobile device
6. Finance to view fuel usage, mileage, and maintenance cost reports per vehicle

## Your Task

Design a software architecture for TrackFleet that addresses the problems above.

Your design should consider:
- How to ingest continuous location and engine data from 600 devices simultaneously without data loss
- How to detect and alert on a route deviation or delivery delay in near-real time
- What happens to data collected by a truck when it enters a zone with no mobile network coverage
- How to store months of historical vehicle telemetry efficiently for maintenance trend analysis
