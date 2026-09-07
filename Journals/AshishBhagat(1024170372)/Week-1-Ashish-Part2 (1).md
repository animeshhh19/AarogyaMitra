Week 1 Project Journal — ArogyaMitra: AI-Assisted Real-Time Telemedicine Consultation Platform

Week 1 — Ideation, Research and Project Proposal (Part 2: Backend, Database and Auth)

| Field | Details |
|---|---|
| Course | UCS503 / UCS503P — Software Engineering |
| Institute | Thapar Institute of Engineering and Technology, Patiala |
| Project | ArogyaMitra: An AI-Assisted Real-Time Telemedicine Consultation Platform |
| Member | Ashish Bhagat — 1024170372 |
| Team Members | Animesh Sudhanshu — 1024170375, Ashish Bhagat — 1024170372, Devansh Rathaur — 1024170380 |
| My Part | Part 2 — Backend, Database and Auth |
| Project Stage | Project Proposal |
| Week | Week 1 of 13 |

Objective for the Week

The objective of Week 1 was to understand the backend, data storage, and authentication requirements of the platform, research an existing open-source reference implementation, and contribute the backend-related sections to the project proposal.

Day 1 — Problem Understanding

Analysed the backend-side pain points described in the problem statement, for example fragmented communication with no persistent record, and no easy way for patients to track booking status or doctor availability.

Looked at what a REST API and a proper database would need to solve for: persistent appointment records, consultation history, and a single source of truth for doctor availability.

Day 2 — Existing Systems and Research

Studied the reference open-source implementation to see how it structures its backend, for example its use of Node.js and Express for the API layer and MongoDB Atlas for storage.

Reviewed how Firebase Authentication is used in that project for both patient and doctor accounts, to understand whether we could reuse the same approach.

Day 3 — Data Model Research

Sketched an initial data model covering users, appointments, consultation notes, and message history, based on what the proposal's core workflow needs.

Compared a few approaches for representing doctor availability in MongoDB, for example fixed time slots versus open availability windows, and noted the trade-offs for query complexity.

Day 4 — API and Auth Planning

Outlined the REST endpoints needed for the first iteration, for example registration and login, doctor discovery, and appointment booking.

Researched Firebase Authentication's server-side verification flow so the Express backend can validate a request as coming from an authenticated patient or doctor.

Day 5 — CI/CD Research

Researched GitHub Actions for running lint and unit tests automatically on every change, since the proposal calls for fast, safe iterations.

Looked into deployment options suited to a pilot project, for example Render for the backend and Netlify for the frontend, and how a single pipeline could push to both.

Day 6 — Proposal Finalisation

Finalised my sections of the proposal with the team, covering the backend API, MongoDB Atlas schema, Firebase Authentication, and the CI/CD approach.

Reviewed the proposal for consistency between the backend section and the real-time/AI sections, for example making sure appointment records would carry the fields needed for TTC measurement.

Week 1 Deliverables

Studied a working reference implementation's backend, database, and auth setup.

Drafted an initial data model for users, appointments, consultation notes, and message history.

Outlined the first-iteration REST API endpoints and the Firebase Authentication flow.

Researched the CI/CD approach using GitHub Actions, Render, and Netlify.

Contributed my sections to the finalised project proposal.

Individual Contribution

My primary contribution this week was on Part 2 — the backend API, database, and authentication design. I researched the reference implementation's backend structure, drafted the initial MongoDB data model, planned the first-iteration API endpoints and Firebase Authentication flow, and researched the CI/CD approach for the project.

Note: The backend API, database schema, and authentication flow discussed during Week 1 are proposed designs for the upcoming iteration and were not implemented during Week 1, which was focused on ideation, research, and the project proposal.
