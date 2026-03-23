# Case Study 2: Hospital Patient Management System — "MediCore"

## Background

MediCore is a mid-sized private hospital with 400 beds, 20 departments, and over 300 staff including doctors, nurses, and administrative personnel. The hospital currently manages patient records using a mix of paper forms and disconnected spreadsheets. It is planning to replace everything with a unified digital system.

## The Organisation

- **Patients** register, book appointments, and access medical history
- **Doctors** view patient records, write prescriptions, and request lab tests
- **Nurses** update vital signs and administer medications
- **Lab technicians** receive test requests and upload results
- **Admin staff** handle billing, insurance claims, and bed allocation
- **Hospital management** monitors operations and generates reports

## Current Situation

The hospital handles around 800 outpatient visits and 50 emergency admissions per day. Patient data is scattered across departments with no shared access. Doctors often make decisions without seeing complete patient history. Lab results are delivered by paper and frequently delayed.

**Known problems:**
- No centralised patient record — departments cannot share information
- Appointment scheduling is done by phone, leading to double-bookings
- Medication errors occur because nurses cannot verify active prescriptions digitally
- Billing is slow because it requires manual collection of charges from each department
- No audit trail for who accessed or changed a patient's record

## What the System Needs to Do

The new system must allow:

1. Patients to register, book appointments, and view their own records
2. Doctors to access full patient history, write digital prescriptions, and request tests
3. Nurses to record vitals and confirm medication administration
4. Lab technicians to receive test orders and upload results directly to the patient record
5. Admin staff to generate bills automatically from treatment records and submit insurance claims
6. Management to view real-time occupancy, staff workload, and financial reports

## Your Task

Design a software architecture for MediCore that addresses the problems above.

Your design should consider:
- How to keep patient data private and accessible only to authorised roles
- What happens if the system goes offline during an emergency
- How to ensure that any change to a patient record is traceable
- How the system can grow to support additional hospital branches in the future
