# Case Study 13: Multiplayer Online Gaming Platform — "ArenaX"

## Background

ArenaX is an online gaming company that operates a competitive multiplayer game played by 2 million registered users worldwide. Players compete in real-time matches, earn rankings, and purchase in-game items. The game must feel fast and fair — any lag or unfair advantage destroys the player experience.

## The Organisation

- **Players** create accounts, join matches, play games, and purchase cosmetic items
- **Game servers** host active matches and enforce game rules
- **Matchmaking system** groups players of similar skill into fair matches
- **Anti-cheat team** reviews flagged accounts and bans cheaters
- **Game developers** release updates, new content, and patches

## Current Situation

ArenaX runs around 50,000 concurrent players during peak times (evenings and weekends). Players are spread across Asia, Europe, and North America. The current infrastructure is hosted entirely in one data centre in Europe, which creates high latency for players in other regions.

**Known problems:**
- Players in Asia and North America experience noticeable lag (200–400ms) which makes the game unfair
- Matchmaking sometimes places players with very different skill levels together, leading to one-sided matches
- When a new game update is released, all servers must restart simultaneously, causing a 15-minute downtime
- Players who disconnect mid-match cannot rejoin — the match is voided, which frustrates other players
- Cheating software is detected days after becoming widespread, giving cheaters an advantage for too long

## What the System Needs to Do

The new system must allow:

1. Players to log in, view their profile, ranking, and match history
2. The matchmaking system to group players of similar skill for a fair match
3. Real-time gameplay between matched players with minimal latency
4. Players who disconnect to rejoin a match in progress
5. Players to purchase in-game cosmetic items through a secure payment flow
6. Game developers to deploy updates to servers without taking the entire platform offline

## Your Task

Design a software architecture for ArenaX that addresses the problems above.

Your design should consider:
- How to reduce latency for players who are geographically distant from the servers
- How to deploy game updates with zero or minimal downtime
- How to detect cheating behaviour early and with minimal false positives
- How to keep the match state consistent if a player disconnects and reconnects
