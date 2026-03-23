# Case Study 15: Real Estate Listing Platform — "NestFinder"

## Background

NestFinder is an online platform where property owners and real estate agents list properties for sale or rent, and buyers or tenants search for properties. The platform covers residential and commercial properties across a country of 20 million people.

## The Organisation

- **Property seekers** search listings, save favourites, and contact agents or owners
- **Real estate agents** manage listings on behalf of property owners
- **Private owners** list their own properties without an agent
- **NestFinder admin** verifies listings, removes fraudulent posts, and manages subscriptions
- **Mortgage advisors** (partners) advertise their services to buyers viewing listings

## Current Situation

NestFinder has 180,000 active listings and receives around 300,000 search queries per day. Property listings include many photos and sometimes virtual tour videos. The platform is especially popular on weekends when most people browse properties.

**Known problems:**
- Property photos take a long time to load, particularly on mobile
- Listings sometimes show properties that have already been sold or rented, because agents do not update them promptly
- Search results include no map view — users cannot see where properties are relative to schools, transport, or their workplace
- Agents can only access their own listings and cannot track which listings have attracted interest
- There is no way for a property seeker to be notified when a new listing matches their saved search criteria

## What the System Needs to Do

The new system must allow:

1. Property seekers to search by location, property type, price, and features
2. Property seekers to view listings on a map alongside points of interest
3. Agents and owners to create and manage listings including photos and virtual tours
4. Property seekers to save search criteria and receive alerts when a matching new listing appears
5. Agents to see how many views and enquiries each listing has received
6. Admin to verify listings and deactivate ones that have been sold or are fraudulent

## Your Task

Design a software architecture for NestFinder that addresses the problems above.

Your design should consider:
- How to store and serve large numbers of high-resolution photos and videos efficiently
- How to implement location-based search at scale across hundreds of thousands of listings
- How to notify users quickly when a new listing matches their saved search
- How to keep listing status (available, sold, rented) accurate in near-real time
