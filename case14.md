# Case Study 14: Job Recruitment Portal — "HireLink"

## Background

HireLink is an online recruitment platform connecting job seekers with employers. Employers post job vacancies, review applications, and schedule interviews. Job seekers create profiles, upload CVs, and apply for roles. The platform currently serves 50,000 employers and 800,000 job seeker profiles.

## The Organisation

- **Job seekers** create profiles, upload CVs, search for jobs, and apply
- **Employers** post vacancies, review applicants, and manage the hiring pipeline
- **Recruitment agencies** post on behalf of multiple employer clients
- **HireLink admin** handles account verification, reported abuse, and premium subscriptions

## Current Situation

HireLink receives around 20,000 new job applications per day. During major hiring seasons (January and September), this doubles. The platform's matching and search features are basic — job seekers must manually browse and filter, and employers receive many unqualified applications.

**Known problems:**
- Job search results are not personalised — all job seekers see the same results for the same keywords
- Employers are overwhelmed by large volumes of irrelevant applications for each vacancy
- CV uploads fail for files above 2MB despite the stated 5MB limit
- Job seekers have no visibility into where their application is in the process after submitting
- Employer accounts are sometimes created by fake companies posting fraudulent job ads

## What the System Needs to Do

The new system must allow:

1. Job seekers to build a profile, upload a CV, and apply for jobs with one click
2. Job seekers to search for roles by keyword, location, salary, and category
3. Employers to post vacancies and define required qualifications
4. The system to rank applicants by relevance to the job requirements
5. Employers to move applicants through stages (applied, reviewed, interview, offer) and notify them at each stage
6. HireLink admin to verify employer accounts and remove fraudulent listings

## Your Task

Design a software architecture for HireLink that addresses the problems above.

Your design should consider:
- How to match job seekers to relevant roles and surface personalised results
- How to handle large file uploads (CVs, cover letters) reliably
- How to verify that employer accounts represent legitimate organisations
- How to notify job seekers of application status changes without overwhelming them with emails
