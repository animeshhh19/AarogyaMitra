Week 5 Project Journal — ArogyaMitra: AI-Assisted Real-Time Telemedicine Consultation Platform

Week 5 — Consultation Lifecycle, Medical Records and Security Hardening (Part 2: Backend, Database and Auth)

| Field | Details |
|---|---|
| Course | UCS503 / UCS503P — Software Engineering |
| Institute | Thapar Institute of Engineering and Technology, Patiala |
| Project | ArogyaMitra: An AI-Assisted Real-Time Telemedicine Consultation Platform |
| Member | Ashish Bhagat — 1024170372 |
| Team Members | Animesh Sudhanshu — 1024170375, Ashish Bhagat — 1024170372, Devansh Rathaur — 1024170380 |
| My Part | Part 2 — Backend, Database and Auth |
| Project Stage | Second Iteration — Lifecycle, Records and Hardening |
| Week | Week 5 of 13 |

Objective for the Week

The objective of Week 5 was to complete the consultation lifecycle on the backend, add medical records and the data needed by the AI assistant, harden the API, and build the analytics endpoints flagged in earlier weeks.

Day 1 — Consultation Lifecycle and Auto-Close

Defined the consultation lifecycle clearly as pending, in-progress, completed and canceled, with a complete action available to either participant.

Added an hourly scheduled job that closes past consultations, for example marking a joined consultation as completed and a never-joined one as canceled once the booked hour has passed.

Day 2 — Medical Records

Built the medical records endpoints so a patient can upload and view records, and a doctor can view the records of a patient they have a consultation with.

Extended the patient profile with health fields such as blood type, allergies, chronic conditions, current medications and an emergency contact.

Day 3 — Records Sync for the AI Assistant

Worked with the real-time and AI teammate on the data the assistant needs, and added an embedding service that syncs a patient's profile and records into a patient-scoped vector index whenever they change.

Added the AI usage and conversation collections, including an hourly usage counter that expires automatically, so the assistant's quota can be enforced.

Day 4 — Security Hardening

Added standard HTTP security headers, input sanitisation against query injection, and rate limiting on the API.

Tightened request validation across all routes and made sure error responses use consistent status codes, for example 401 for unauthenticated and 403 for unauthorised requests.

Day 5 — Analytics Endpoints

Built the admin analytics endpoints for bookings, booking completion rate and time-to-connect, computed from the stored consultation and join timestamps.

Added tests for the consultation notes endpoints, which were flagged as a coverage gap in Week 3, and for the auto-close job.

Day 6 — Integration and Review

Did a joint test with the team across the full flow, for example booking and paying, joining inside the booked hour, completing the consultation, and confirming the auto-close job and the analytics numbers reflected it correctly.

Reviewed CI results and the staging deployment on Render, and logged the remaining backend work: final end-to-end testing and fixes from the pilot.

Week 5 Deliverables

Consultation lifecycle with an hourly auto-close job.

Medical records endpoints and extended patient health profile.

Embedding sync service and AI usage and conversation collections.

Security hardening: headers, input sanitisation, rate limiting and consistent validation.

Admin analytics endpoints and additional unit tests, all running in CI.

Individual Contribution

This week I completed the remaining core backend features for Part 2: the consultation lifecycle with automatic closing, medical records, the data layer for the AI assistant, security hardening, and the analytics endpoints used to measure time-to-connect and booking completion rate.

Note: The pilot with test users and the final end-to-end testing and fixes are not yet done, Week 5 focused on completing the remaining backend features. These are planned for the coming weeks per the proposal's iteration plan.
