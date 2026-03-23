# Case Study 1: Online Food Delivery Platform — "QuickBite"

## Background

QuickBite is a startup food delivery company operating in a mid-sized city. It connects customers with local restaurants and independent delivery drivers through a mobile app and website.

The company currently has a working but struggling system. As the business grows, the team has identified several problems they need you to solve through good software architecture.

## The Organisation

- **Customers** browse menus, place orders, and pay online
- **Restaurant partners** receive orders and update preparation status
- **Delivery drivers** (independent contractors) pick up and deliver orders
- **Operations team** monitors orders and handles complaints

## Current Situation

QuickBite processes around 5,000 orders per day. The system works fine during quiet periods but struggles during lunch and dinner rush hours. The company plans to expand to 3 more cities within the next year.

**Known problems:**
- The system becomes slow or crashes during peak hours
- Restaurants sometimes receive order notifications late
- Customers have no way to track where their delivery is
- Managing driver payments is done manually and takes days

## What the System Needs to Do

The new system must allow:

1. Customers to search restaurants, browse menus, and place orders
2. Restaurants to receive and manage incoming orders
3. The system to automatically assign a nearby driver to each confirmed order
4. Customers to track their order delivery in real time
5. Online payment processing
6. Drivers and restaurants to view their earnings

## Your Task

Design a software architecture for QuickBite that addresses the problems above and supports the company's growth plans.

Your design should consider:
- What could go wrong at peak times and how to handle it
- What happens when the company scales to 4× the current load
- How sensitive data (payments, user accounts) should be protected
- How easy it should be to add new features in the future
