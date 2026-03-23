# Case Study 22: Public Library Management System — "LibraNet"

## Background

LibraNet is a digital management system for a network of 35 public libraries operated by a city council. The system manages physical book collections, member accounts, borrowing and returns, reservations, and fines. The council also wants to add an e-book lending service that allows members to borrow digital titles through the app.

## The Organisation

- **Library members** search the catalogue, borrow and return books, reserve items, and borrow e-books
- **Library staff** check in returned items, process reservations, and assist members
- **Head librarians** manage the catalogue, set borrowing policies, and track collection usage
- **City council finance** tracks fine collection and budget allocation per branch

## Current Situation

Each of the 35 branches currently uses a standalone system with its own catalogue. A member registered at one branch cannot borrow from another without re-registering. There is no shared catalogue, meaning members cannot search availability across all branches at once.

**Known problems:**
- A member cannot see or reserve a book that is available at a different branch
- When a book is returned to the wrong branch, it takes several days to be tracked and returned to the correct catalogue
- Fine notices are sent by post and many go uncollected because members have moved address
- E-books are managed through a separate third-party system with no connection to the main membership database
- Staff spend significant time manually processing reservation queues when popular books become available

## What the System Needs to Do

The new system must allow:

1. Members to search the combined catalogue across all 35 branches
2. Members to reserve a book at any branch and be notified when it is ready for collection
3. Members to borrow and return items at any branch, not just their home branch
4. Members to borrow e-books through the app up to their borrowing limit
5. Staff to process returns, reservations, and renewals efficiently
6. The system to automatically notify members of overdue items and outstanding fines

## Your Task

Design a software architecture for LibraNet that addresses the problems above.

Your design should consider:
- How to unify 35 separate catalogues into a single searchable system without losing branch-level information
- How to manage the limited number of simultaneous e-book licences (publishers often restrict concurrent borrows)
- How to automate the reservation queue fairly when multiple members are waiting for the same book
- How to reach members through multiple channels (email, SMS, app notification) for overdue and fine alerts
