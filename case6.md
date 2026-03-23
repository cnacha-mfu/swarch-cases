# Case Study 6: University Learning Management System — "CampusLearn"

## Background

A university with 25,000 students and 1,200 academic staff currently uses a combination of email, shared drives, and a very outdated portal to manage course delivery. The university wants to replace these with a modern Learning Management System (LMS) that handles everything from content delivery to assessments and grades.

## The Organisation

- **Students** access course materials, submit assignments, and sit online exams
- **Lecturers** upload content, set assignments, grade submissions, and communicate with students
- **Course coordinators** manage course enrolments and track academic progress
- **IT administrators** manage user accounts and system access
- **University management** accesses academic performance reports

## Current Situation

The university runs two semesters per year. At the start of each semester, around 20,000 students log in within the first few days, causing the current portal to slow down significantly. Final exam periods create similar spikes.

**Known problems:**
- Large video lectures cannot be uploaded reliably — uploads frequently fail
- Students can access course pages they are not enrolled in
- Assignment submissions sometimes disappear or are not recorded
- Lecturers cannot see at a glance which students have fallen behind
- Plagiarism between submissions is not automatically detected

## What the System Needs to Do

The new system must allow:

1. Lecturers to create courses and upload materials (videos, documents, slides)
2. Students to access only the courses they are enrolled in
3. Students to submit assignments online before a deadline
4. Lecturers to grade submissions and return feedback digitally
5. The system to flag potentially plagiarised submissions for lecturer review
6. Students and lecturers to communicate through announcements and messaging
7. Coordinators to view progress reports per student and per course

## Your Task

Design a software architecture for CampusLearn that addresses the problems above.

Your design should consider:
- How to handle large file uploads reliably without failing mid-way
- How to manage access so students only see courses they are enrolled in
- How to ensure assignment submissions are never lost
- How to keep the system responsive during semester start and exam periods
