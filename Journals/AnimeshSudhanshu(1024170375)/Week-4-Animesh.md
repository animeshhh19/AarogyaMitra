Week 4 Project Journal — ArogyaMitra: AI-Assisted Real-Time Telemedicine Consultation Platform

Week 4 — Video Consultation UI, Payments and Alerts (Part 1: Frontend and Patient/Doctor Portal)

| Field | Details |
|---|---|
| Course | UCS503 / UCS503P — Software Engineering |
| Institute | Thapar Institute of Engineering and Technology, Patiala |
| Project | ArogyaMitra: An AI-Assisted Real-Time Telemedicine Consultation Platform |
| Member | Animesh Sudhanshu — 1024170375 |
| Team Members | Animesh Sudhanshu — 1024170375, Ashish Bhagat — 1024170372, Devansh Rathaur — 1024170380 |
| My Part | Part 1 — Frontend and Patient/Doctor Portal |
| Project Stage | Second Iteration — Approval, Payments and Video Access |
| Week | Week 4 of 13 |

Objective for the Week

The objective of Week 4 was to build the video consultation screen, add the payment step to the booking flow for paid doctors, and add in-app consultation alerts on top of the core booking, queue, history and chat screens from Week 3.

Day 1 — Authentication Pages Update

Updated the sign-in and sign-up pages to use the Clerk Next.js SDK, so the frontend gets a session token that the backend now verifies.

Added role-aware redirects after sign-in, for example sending a patient, doctor or admin to their own portal.

Day 2 — Video Consultation Screen

Built the consultation room screen using the video room components provided by the real-time layer, with the video tiles and the chat panel together on one page.

Added UI states for joining, waiting for the other participant, and connection problems, so a user knows what is happening before the doctor or patient arrives.

Day 3 — Join Window in the UI

Added the join button logic so a consultation can be joined only inside the booked hour, with a clear message before the slot starts and after it has passed.

Handled the case where the backend rejects a join, for example showing a readable error instead of a blank room.

Day 4 — Payment Flow

Added the payment step to the booking flow for paid doctors, redirecting to Stripe Checkout and returning to a confirmation page, while free doctors continue to book directly.

Handled the cancelled and failed payment returns, for example showing the booking as not confirmed and letting the patient retry.

Day 5 — Consultation Alerts and Doctor Price Display

Built the in-app consultation alerts for doctors and patients, using the existing polling approach so the alert appears when a consultation is about to begin.

Showed the consultation fee on the doctor discovery cards and the booking screen so the patient knows the cost before checkout.

Day 6 — Integration and Review

Did a joint test with the team across the paid booking, the free booking, the alert, and joining the video room from both the patient and the doctor side.

Checked the new screens on smaller viewports and logged the remaining frontend work: the admin portal, the AI assistant chat screen and the medical records pages.

Week 4 Deliverables

Sign-in and sign-up pages updated to Clerk with role-aware redirects.

Video consultation screen with chat panel and join, waiting and error states.

Join window handling in the UI.

Payment step with Stripe Checkout return handling.

In-app consultation alerts and fee display on doctor cards.

Individual Contribution

This week I extended Part 1 from the core booking, queue, history and chat screens to the full consultation experience: updated authentication pages, the video consultation screen, join window handling, the Stripe payment step and in-app consultation alerts.

Note: The admin portal, the AI assistant chat screen, the medical records pages and the analytics views are not yet built, Week 4 focused on video, payments and alerts. These are planned for the coming weeks per the proposal's iteration plan.
