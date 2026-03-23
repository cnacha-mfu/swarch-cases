# Case Study 16: Video Streaming Service — "StreamVault"

## Background

StreamVault is a subscription-based video streaming service offering a library of 15,000 movies and TV series. Subscribers pay a monthly fee and can watch content on any device — smart TV, phone, tablet, or browser. The service operates in 12 countries and streams in multiple languages with subtitles.

## The Organisation

- **Subscribers** browse the catalogue, watch content, and manage their accounts
- **Content team** uploads new titles, adds metadata, and manages the content library
- **Rights management team** controls which content is available in which country
- **Analytics team** tracks viewing behaviour to improve recommendations
- **Finance team** manages subscriptions, billing, and refunds

## Current Situation

StreamVault has 4 million active subscribers. Peak viewing is between 7 PM and 11 PM on weekdays, and most of the day on weekends. During these peaks, the service must deliver smooth video to hundreds of thousands of simultaneous streams.

**Known problems:**
- Video playback frequently buffers during peak evening hours
- New content uploads take 24–48 hours to be available because video processing is slow
- The recommendation engine suggests the same popular titles to everyone rather than personalising to viewing history
- Subtitles are sometimes out of sync with the video
- Users who travel abroad find that content they were watching at home is blocked

## What the System Needs to Do

The new system must allow:

1. Subscribers to browse and search the content library
2. Subscribers to stream video smoothly at varying quality depending on internet speed
3. Content team to upload a video and have it available to stream within a few hours
4. The system to display content appropriate to the subscriber's country (geo-restrictions)
5. The recommendation engine to suggest content personalised to each subscriber's viewing history
6. Subscribers to download content for offline viewing within their subscription tier

## Your Task

Design a software architecture for StreamVault that addresses the problems above.

Your design should consider:
- How to deliver video to hundreds of thousands of concurrent viewers without buffering
- How to process and encode uploaded videos quickly into multiple quality formats
- How to store and serve 15,000 titles' worth of video data cost-effectively
- How to personalise recommendations for millions of users at scale
