Week 4 Project Journal — ArogyaMitra: AI-Assisted Real-Time Telemedicine Consultation Platform

Week 4 — Doctor Approval, Payments and Consultation Access Control (Part 2: Backend, Database and Auth)

| Field | Details |
|---|---|
| Course | UCS503 / UCS503P — Software Engineering |
| Institute | Thapar Institute of Engineering and Technology, Patiala |
| Project | ArogyaMitra: An AI-Assisted Real-Time Telemedicine Consultation Platform |
| Member | Ashish Bhagat — 1024170372 |
| Team Members | Animesh Sudhanshu — 1024170375, Ashish Bhagat — 1024170372, Devansh Rathaur — 1024170380 |
| My Part | Part 2 — Backend, Database and Auth |
| Project Stage | Second Iteration — Approval, Payments and Video Access |
| Week | Week 4 of 13 |

Objective for the Week

The objective of Week 4 was to extend the backend beyond the core booking loop: add admin approval of doctors, integrate Stripe payments for paid doctors, and enforce who can join a consultation and when.

Day 1 — Authentication Update and Doctor Approval

Replaced the earlier token verification with Clerk JWT verification middleware, so protected routes identify the requesting patient, doctor or admin from the Clerk session token, and a MongoDB user record is created on first sign-in.

Added an approval status to doctor profiles, for example pending by default on signup, with approved and rejected as the other states.

Day 2 — Admin Endpoints

Built the admin endpoints for listing pending doctors, approving or rejecting a doctor, and managing patient accounts.

Added an admin check middleware so these routes are reachable only by users with the admin role, and made doctor discovery return approved doctors only.

Day 3 — Stripe Checkout

Added a Payment model storing the Stripe session, amount, status, and the patient, doctor and consultation references.

Built the checkout session endpoint for paid doctors, while free doctors continue to book directly without a payment step.

Day 4 — Payment Fulfilment

Implemented the Stripe webhook handler for completed checkout sessions, along with a confirm-payment endpoint as a fallback if the webhook is delayed.

Made fulfilment idempotent, so only a payment that is not yet paid can flip to paid once and create the consultation, which prevents duplicate bookings from repeated webhook calls.

Day 5 — Consultation Access Control

Connected the consultation routes to the video room service built by the real-time teammate, for example issuing a room access token only to the booked patient or doctor.

Enforced the booked-hour join window, so a participant can join only inside the booked clock-hour, and marked the consultation in-progress on the first valid join.

Day 6 — Integration and Review

Did a joint test with the team across the paid booking flow, the free booking flow, doctor approval, and joining a consultation inside and outside the booked hour.

Added unit tests for the approval flow and for idempotent payment fulfilment, and logged the remaining backend work for next week: automatic closing of past consultations, medical records, and security hardening.

Week 4 Deliverables

Clerk JWT verification middleware and user record sync on first sign-in.

Doctor approval status with admin approve and reject endpoints.

Stripe checkout, webhook and confirm-payment endpoints with idempotent fulfilment.

Consultation join control based on participant check and the booked-hour window.

Unit tests for approval and payment fulfilment running in the CI pipeline.

Individual Contribution

This week I extended Part 2 from the core booking loop to the full paid consultation path: updated the authentication middleware, built the doctor approval and admin endpoints, integrated Stripe checkout with idempotent fulfilment, and enforced participant and time-window checks before a consultation room can be joined.

Note: Automatic closing of past consultations, medical records, security hardening and the admin analytics endpoints are not yet built, Week 4 focused on approval, payments and join control. These are planned for the coming weeks per the proposal's iteration plan.
