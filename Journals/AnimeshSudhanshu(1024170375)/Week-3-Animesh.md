Week 3 Project Journal — ArogyaMitra: AI-Assisted Real-Time Telemedicine Consultation Platform

Week 3 — Booking Flow Completion and Consultation UI (Part 1: Frontend and Patient/Doctor Portal)

| Field | Details |
|---|---|
| Course | UCS503 / UCS503P — Software Engineering |
| Institute | Thapar Institute of Engineering and Technology, Patiala |
| Project | ArogyaMitra: An AI-Assisted Real-Time Telemedicine Consultation Platform |
| Member | Animesh Sudhanshu — 1024170375 |
| Team Members | Animesh Sudhanshu — 1024170375, Ashish Bhagat — 1024170372, Devansh Rathaur — 1024170380 |
| My Part | Part 1 — Frontend and Patient/Doctor Portal |
| Project Stage | First Iteration — Core Consultation Loop |
| Week | Week 3 of 13 |

Objective for the Week

The objective of Week 3 was to complete the appointment booking flow on the frontend, build the doctor's appointment queue view, and put together the first version of the consultation chat screen.

Day 1 — Appointment Booking Completion

Finished the appointment booking flow end to end, for example showing a clear confirmation screen once a slot is booked and reflecting pending, confirmed, and completed statuses correctly.

Handled edge cases in the UI, for example a doctor cancelling availability after a patient had already selected that slot.

Day 2 — Doctor Appointment Queue

Built the doctor's appointment queue view, showing upcoming and past appointments with their current status.

Added simple filtering and sorting on the queue, for example by date or status, so a doctor can quickly see what is coming up next.

Day 3 — Consultation History Pages

Built the consultation history page on the patient side, so a patient can review past consultations and any notes left by the doctor.

Added pagination on the history list to match the backend's paginated endpoint.

Day 4 — Consultation Chat Screen

Built the first version of the consultation chat screen, wiring it up to the real-time layer's Socket.io events for sending and receiving messages.

Added basic UI states for connection status, for example showing when the other participant has joined the room.

Day 5 — Responsive and Device Testing

Tested the patient portal and doctor dashboard on a few lower-end device profiles and smaller screen sizes, adjusting layout and component sizing where needed.

Fixed a few responsiveness issues on the booking flow and chat screen that only showed up on smaller viewports.

Day 6 — Integration and Review

Did a joint test with the team across the booking flow, appointment queue, consultation history, and chat screen, for example booking a slot, confirming it appeared correctly in the doctor's queue, and exchanging messages once the room opened.

Reviewed the UI against the CI pipeline's staging deployment to confirm the frontend build was deploying correctly through Netlify.

Logged remaining frontend work for upcoming weeks: integrating the video call UI once WebRTC is wired up, and building the admin and analytics views.

Week 3 Deliverables

Completed appointment booking flow with status display and edge case handling.

Doctor appointment queue view with filtering and sorting.

Consultation history page with pagination on the patient side.

First version of the consultation chat screen connected to the real-time layer.

Responsiveness fixes for lower-end devices and smaller screens.

Individual Contribution

This week I completed the core Part 1 deliverables for the first iteration: the appointment booking flow, the doctor's appointment queue, the consultation history page, and the first working version of the consultation chat screen, along with responsiveness fixes across the portal.

Note: The video call UI and the admin and analytics views are not yet built, Week 3 focused on completing the core booking, queue, history, and chat screens. These are planned for upcoming weeks per the proposal's iteration plan.
