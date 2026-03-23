# Case Study 18: Government e-Services Portal — "CitizenGate"

## Background

CitizenGate is a national digital government initiative to bring public services online. Citizens can apply for identity documents, pay government fees, renew licences, and access social services through a single portal. The system replaces in-person visits to multiple government offices.

## The Organisation

- **Citizens** apply for services, upload documents, pay fees, and track application status
- **Government clerks** review applications, request additional documents, and approve or reject requests
- **Multiple government agencies** each own a set of services (e.g., Transport Authority, Civil Registry, Tax Department)
- **System administrators** manage access control and monitor the platform
- **Auditors** review government decisions and access logs

## Current Situation

Each government agency currently runs its own separate system with different login credentials, different document requirements, and different processing times. Citizens must visit each agency separately for services that require coordination between agencies.

**Known problems:**
- Citizens must upload the same identity documents repeatedly to different agencies
- There is no way to track an application once submitted — citizens must call or visit to follow up
- Some application forms are still only available as downloadable PDFs that must be printed and scanned
- Processing times vary widely and there is no standard service level agreement across agencies
- The system has no way to verify whether a submitted document is authentic

## What the System Needs to Do

The new system must allow:

1. Citizens to create a single verified digital identity used across all government services
2. Citizens to submit applications for services from any agency through one portal
3. Citizens to upload supporting documents once and re-use them across multiple applications
4. Citizens to track the status of their application in real time
5. Government clerks to review, approve, or reject applications and request additional documents
6. Agencies to define their own workflows, forms, and document requirements within the portal

## Your Task

Design a software architecture for CitizenGate that addresses the problems above.

Your design should consider:
- How to verify a citizen's identity securely during registration
- How to integrate multiple agencies with different processes without tightly coupling them
- How to ensure that sensitive personal data is accessible only to the agencies and clerks who need it
- How to maintain a complete audit trail of every action taken on every application
