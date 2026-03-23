# Case Study 7: Smart City Traffic Management System — "FlowCity"

## Background

FlowCity is a government initiative to reduce traffic congestion in a capital city of 3 million people. The city has installed sensors and cameras at 800 intersections. The goal is to use this data to control traffic signals intelligently, detect incidents, and provide real-time information to drivers.

## The Organisation

- **Traffic control centre operators** monitor the city, override signals manually in emergencies
- **City planners** analyse traffic patterns and plan road infrastructure
- **Emergency services** (police, ambulance, fire) need traffic lights to be cleared on their route
- **Drivers** receive route guidance through navigation apps via a public data feed
- **City IT team** maintains the system infrastructure

## Current Situation

The existing system was installed 15 years ago. Signal timings are fixed and do not adapt to actual traffic conditions. Incidents such as accidents or broken-down vehicles are only reported when a driver or pedestrian calls the control centre. There is no automated detection.

**Known problems:**
- Fixed signal timings cause unnecessary congestion during off-peak hours and do not clear during gridlock
- Incident detection relies entirely on phone calls, often causing 15–30 minute delays in response
- Emergency vehicles are often stuck in traffic with no way to request signal clearance ahead
- Sensor and camera data is not centralised — each intersection operates independently
- There is no historical data for traffic pattern analysis

## What the System Needs to Do

The new system must allow:

1. Sensors and cameras at each intersection to stream traffic data to a central system in real time
2. The system to automatically adjust signal timings based on current traffic density
3. Operators to view a live city-wide traffic map and manually override any signal
4. Automatic detection of incidents (stopped vehicles, unusual congestion) and alerting of operators
5. Emergency services to request a cleared signal corridor from their current location to their destination
6. Historical traffic data to be stored and made available for analysis and reporting

## Your Task

Design a software architecture for FlowCity that addresses the problems above.

Your design should consider:
- How to process a continuous stream of sensor data from 800 locations in real time
- What happens if the central system or a network link goes down — can intersections operate independently?
- How to prioritise emergency vehicle requests above all other signal decisions
- How to store large volumes of historical sensor data efficiently for future analysis
