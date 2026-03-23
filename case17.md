# Case Study 17: Fitness & Health Tracking App — "PulseFit"

## Background

PulseFit is a mobile fitness app that helps users track workouts, monitor health metrics, and follow personalised training plans. The app integrates with wearable devices (smartwatches and fitness bands) to collect data such as heart rate, steps, sleep, and calories. It has 1.2 million active users.

## The Organisation

- **Users** log workouts, view health data, and follow training plans
- **Certified coaches** (partners) create and sell training plans through the platform
- **Device manufacturers** (partners) integrate their wearables with PulseFit via an API
- **PulseFit health team** reviews the scientific basis of training content
- **Premium subscribers** pay for advanced analytics and access to coach plans

## Current Situation

PulseFit syncs data from wearables every few minutes throughout the day. Over time, each user accumulates a large personal dataset. The app currently stores all raw sensor data indefinitely, which is creating storage and performance problems.

**Known problems:**
- Syncing data from some wearable brands is unreliable — data frequently comes in duplicate or out of order
- The health dashboard is slow to load because it recalculates all metrics from raw data each time
- Users who change their phone or wearable lose their historical data
- Coach-created training plans are not personalised — every user on a plan gets the same programme regardless of their current fitness level
- There is no way for users to export their health data or delete their account

## What the System Needs to Do

The new system must allow:

1. Wearable devices to sync health data (steps, heart rate, sleep, calories) to the app continuously
2. Users to view daily, weekly, and monthly summaries of their health metrics
3. Users to log manual workouts when not using a wearable
4. Coaches to create and publish training plans that users can subscribe to
5. The system to adjust a training plan's difficulty based on a user's recent performance
6. Users to export their personal data and delete their account on request

## Your Task

Design a software architecture for PulseFit that addresses the problems above.

Your design should consider:
- How to handle data arriving out of order or as duplicates from wearable devices
- How to keep the health dashboard fast despite each user having months or years of historical data
- How to store large volumes of time-series sensor data efficiently and cost-effectively
- How to ensure users own and can control their personal health data
