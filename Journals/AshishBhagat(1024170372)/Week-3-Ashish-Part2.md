Week 3 Project Journal — ArogyaMitra: AI-Assisted Real-Time Telemedicine Consultation Platform

Week 3 — Booking Flow Completion and CI/CD Setup (Part 2: Backend, Database and Auth)

| Field | Details |
|---|---|
| Course | UCS503 / UCS503P — Software Engineering |
| Institute | Thapar Institute of Engineering and Technology, Patiala |
| Project | ArogyaMitra: An AI-Assisted Real-Time Telemedicine Consultation Platform |
| Member | Ashish Bhagat — 1024170372 |
| Team Members | Animesh Sudhanshu — 1024170375, Ashish Bhagat — 1024170372, Devansh Rathaur — 1024170380 |
| My Part | Part 2 — Backend, Database and Auth |
| Project Stage | First Iteration — Core Consultation Loop |
| Week | Week 3 of 13 |

Objective for the Week

The objective of Week 3 was to complete the appointment booking flow end to end, set up the first CI/CD pipeline, and add the logging and query support the rest of the team needs from the backend.

Day 1 — Appointment Booking Completion

Finished the appointment booking endpoint, for example handling edge cases like a doctor cancelling availability after a slot was already booked.

Added confirmation responses and appointment status fields, for example pending, confirmed, and completed, so the frontend can reflect booking state accurately.

Day 2 — Consultation Record Endpoints

Built the endpoints for consultation notes and history, so a doctor can record notes during or after a consultation and a patient can review past consultations from their profile.

Added pagination on the consultation history endpoint since a patient's history could grow over many appointments.

Day 3 — Support for Real-time and TTC Logging

Added the appointment fields and a small logging endpoint needed by the real-time layer, for example exposing the scheduled start time cleanly so TTC can be measured against it.

Coordinated with the teammate handling the real-time layer to confirm the appointment ID and room-naming convention matched on both sides.

Day 4 — CI Pipeline Setup

Set up the first GitHub Actions workflow to run lint and backend unit tests automatically on every push and pull request.

Wrote initial unit tests for the authentication middleware and the appointment booking logic, for example testing that double-booking is correctly rejected.

Day 5 — CD to Staging

Configured deployment of the backend to Render as a staging environment, triggered from the same GitHub Actions pipeline after tests pass.

Verified the staging backend could connect to MongoDB Atlas and Firebase Authentication correctly, separate from the local development setup.

Day 6 — Integration and Review

Did a joint test with the team across the booking flow, real-time chat, and staging deployment, for example booking a slot, confirming the room became accessible at the scheduled time, and checking the appointment status updated correctly.

Reviewed test coverage and flagged gaps for next week, for example adding tests for the consultation notes endpoints.

Logged remaining backend work for upcoming weeks: admin and analytics endpoints for TTC and booking completion rate, and tightening validation across all routes.

Week 3 Deliverables

Completed appointment booking flow with status tracking and double-booking prevention.

Consultation notes and history endpoints with pagination.

Backend fields and logging support for the real-time layer's TTC measurement.

First GitHub Actions pipeline running lint and unit tests on every change.

Backend deployed to a staging environment on Render through the CI/CD pipeline.

Individual Contribution

This week I completed the core Part 2 deliverables for the first iteration: the appointment booking flow, consultation notes and history endpoints, the backend support needed for TTC measurement, and the first CI/CD pipeline with automated tests and staging deployment.

Note: Admin and analytics endpoints for TTC and booking completion rate are not yet built, Week 3 focused on completing the core booking and consultation record flow along with the CI/CD setup. These are planned for upcoming weeks per the proposal's iteration plan.
