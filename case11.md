# Case Study 11: Telemedicine Platform — "DocNow"

## Background

DocNow is a telehealth startup that allows patients to consult with licensed doctors via video call, text chat, or voice call through a mobile app. After a consultation, doctors can issue digital prescriptions that patients can send to any pharmacy. The platform operates across three countries with different healthcare regulations.

## The Organisation

- **Patients** register, book consultations, attend video calls, and receive prescriptions
- **Doctors** (licensed, verified contractors) set their availability, conduct consultations, and issue prescriptions
- **Pharmacies** (partner network) receive and verify digital prescriptions
- **DocNow compliance team** ensures doctors are licensed in the correct country and consultations meet regulatory standards

## Current Situation

DocNow handles around 1,200 consultations per day. Demand spikes in winter when flu season increases the need for quick medical advice. The platform has been growing rapidly through word of mouth but the technical infrastructure has not kept pace.

**Known problems:**
- Video call quality degrades when multiple consultations happen simultaneously
- Patients sometimes wait over 30 minutes before a doctor becomes available, with no queue status updates
- Consultation recordings (required by regulation in two of the three countries) are stored without encryption
- Doctors have accidentally issued prescriptions using another country's prescription format
- There is no way for a doctor to see a patient's previous consultation history on the platform

## What the System Needs to Do

The new system must allow:

1. Patients to select a consultation type (video, voice, or chat) and book an available doctor
2. Patients to be notified of their queue position and estimated wait time
3. Doctors and patients to conduct consultations through the platform
4. Doctors to view a patient's previous consultation history before and during a call
5. Doctors to issue a digital prescription at the end of a consultation
6. Consultation records to be stored securely and accessible to compliance staff

## Your Task

Design a software architecture for DocNow that addresses the problems above.

Your design should consider:
- How to deliver good video call quality even when many consultations are running simultaneously
- How to keep patient health information private and compliant with healthcare data regulations
- How to apply different rules (prescription formats, recording requirements) based on which country the patient and doctor are in
- What happens if a video call drops mid-consultation — can the patient and doctor reconnect without losing context?
