Week 2 Project Journal — ArogyaMitra: AI-Assisted Real-Time Telemedicine Consultation Platform

Week 2 — Environment Setup and Core API Groundwork (Part 2: Backend, Database and Auth)

| Field | Details |
|---|---|
| Course | UCS503 / UCS503P — Software Engineering |
| Institute | Thapar Institute of Engineering and Technology, Patiala |
| Project | ArogyaMitra: An AI-Assisted Real-Time Telemedicine Consultation Platform |
| Member | Ashish Bhagat — 1024170372 |
| Team Members | Animesh Sudhanshu — 1024170375, Ashish Bhagat — 1024170372, Devansh Rathaur — 1024170380 |
| My Part | Part 2 — Backend, Database and Auth |
| Project Stage | Initial Setup and First Iteration |
| Week | Week 2 of 13 |

Objective for the Week

The objective of Week 2 was to move from proposal to practice: set up the backend locally, connect it to MongoDB Atlas, get Firebase Authentication working end to end, and start building out the core API endpoints.

Day 1 — Backend Environment Setup

Set up the Express backend locally from the forked repository, for example configuring environment variables for the database connection and Firebase credentials.

Connected the backend to a MongoDB Atlas cluster and verified the connection with a basic health-check route.

Day 2 — Data Model Implementation

Implemented the initial Mongoose schemas for users, appointments, and consultation notes based on last week's data model draft.

Added basic indexing on frequently queried fields, for example appointment date and doctor ID, to keep lookups fast as data grows.

Day 3 — Firebase Authentication Integration

Wired up Firebase Authentication on the backend, including server-side token verification middleware so protected routes can identify the requesting patient or doctor.

Tested the signup and login flow end to end with a couple of test accounts, for example one patient account and one doctor account.

Day 4 — Core API Endpoints

Built the first set of REST endpoints: user registration and profile, doctor discovery, and doctor availability management.

Added basic request validation and error handling so malformed requests fail with clear messages instead of silent errors.

Day 5 — Appointment Booking Logic

Started implementing the appointment booking endpoint, for example checking a doctor's availability before confirming a slot and preventing double-booking of the same slot.

Discussed with the team how appointment records need to carry the fields the real-time layer depends on, for example the scheduled start time used for TTC measurement.

Day 6 — Integration Check-in and Planning

Did a joint test with the team, registering a patient and doctor account through the actual API and confirming both showed up correctly in MongoDB Atlas.

Reviewed progress against the initial deliverable checklist from the proposal and flagged the booking flow and CI setup as priorities for next week.

Planned next week's work: finish the appointment booking flow and set up the first GitHub Actions pipeline for lint and unit tests.

Week 2 Deliverables

Backend running locally and connected to MongoDB Atlas.

Implemented Mongoose schemas for users, appointments, and consultation notes.

Working Firebase Authentication flow with server-side token verification.

First set of REST API endpoints for registration, profile, doctor discovery, and availability.

Appointment booking logic in progress, including double-booking prevention.

Individual Contribution

This week I moved Part 2 from planning into setup: got the backend running locally and connected to MongoDB Atlas, implemented the core schemas, wired up Firebase Authentication with server-side verification, and built the first set of API endpoints along with the start of the appointment booking logic.

Note: The full booking flow and the CI/CD pipeline are not yet complete, Week 2 focused on environment setup and core API groundwork. These are targeted for completion in the coming weeks per the proposal's iteration plan.
