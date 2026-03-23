# Case Study 9: Social Media Platform — "Connekt"

## Background

Connekt is a social media platform where users share short posts, photos, and short videos, follow other users, and interact through likes and comments. The platform has grown to 5 million registered users in two years and is now experiencing serious performance and moderation challenges.

## The Organisation

- **Users** create profiles, post content, follow others, and interact with posts
- **Content moderators** review reported content and take action on policy violations
- **Advertisers** run targeted ad campaigns based on user interests and demographics
- **Connekt management** monitors platform health, growth, and advertiser revenue

## Current Situation

Connekt generates around 500,000 new posts per day. The news feed — which shows each user a personalised list of posts from the people they follow — is the core feature of the app. As the user base has grown, generating the news feed has become very slow.

**Known problems:**
- News feed takes 5–10 seconds to load for users who follow many accounts
- Uploaded photos and videos sometimes fail mid-upload or take very long to process
- Reported content often stays visible for hours before a moderator reviews it
- Popular posts that go viral cause sudden spikes in read traffic that crash the database
- User account data and browsing activity is stored with no clear policy on what can be used for ads

## What the System Needs to Do

The new system must allow:

1. Users to create posts containing text, photos, or short videos
2. Users to follow other accounts and see a personalised feed of recent posts
3. Users to like, comment on, and share posts
4. Users to report content that violates community guidelines
5. Moderators to review reported content and remove or escalate it
6. Advertisers to create campaigns that target specific user segments

## Your Task

Design a software architecture for Connekt that addresses the problems above.

Your design should consider:
- How to generate personalised news feeds quickly for millions of users
- How to handle the sudden read traffic spike when a post goes viral
- How to process uploaded media (resize images, transcode videos) without blocking the user
- How to handle user data responsibly and make privacy controls clear and enforceable
