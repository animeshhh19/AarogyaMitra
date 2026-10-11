# Week 4 Project Journal — Video Consultation & Room Access Control

## Week 4 — Video Consultation & Room Access Control

### Project Details

| **Course** | UCS503 / UCS503P — Software Engineering |

| **Institute** | Thapar Institute of Engineering and Technology, Patiala |

| **Project** | Telemedicine Platform |

| **Member** | Devansh Rathaur 1024170380 |

| **Team Members** | Ashish Bhagat 1024170372, Devansh Rathaur 1024170380, Animesh Sudhanshu 1024170375 |

| **Project Stage** | Second Iteration — Approval, Payments and Video Access |

| **Week** | Week 4 |

### Objective for the Week

The objective of Week 4 was to add video consultation on top of the Week 3 chat, and to make sure a consultation room can only be joined by the right people at the right time.

### Day 1 — Video Approach Evaluation

Compared building WebRTC signalling over Socket.io with using LiveKit, a managed WebRTC service, for the video rooms.
- Chose LiveKit for the video and chat rooms, since it reduces the signalling and reconnection work and fits the time available.

### Day 2 — LiveKit Setup

Set up a LiveKit project and configured the server keys in the backend environment.
- Created a service that creates a room per consultation, named from the appointment ID.

### Day 3 — Access Token Issue

Built the endpoint that issues a LiveKit access token for a consultation.
- Issued the token only after checking that the user is the booked patient or doctor of that consultation.

### Day 4 — Join Window Check

Added the check that a token is issued only inside the booked hour of the consultation.
- Coordinated with the backend teammate so that the first valid join marks the consultation as in-progress.

### Day 5 — Chat and TTC on LiveKit

Moved the consultation chat to the LiveKit room so that video and chat share one connection.
- Kept the TTC logging by recording the time when both participants are present in the same room.

### Day 6 — Integration and Review

Tested video and chat with the team from both the patient and doctor sides, including joining before and after the booked hour.
- Reviewed reconnection behaviour with the frontend teammate and logged remaining work: the AI assistant and notifications.

### Week 4 Deliverables

- LiveKit based video and chat room per consultation.
- Token endpoint restricted to the booked patient and doctor.
- Join window check based on the booked hour.
- Chat moved to LiveKit with TTC logging kept.
- Tested join flow from both sides.

### Individual Contribution

My primary contribution was adding **video consultation and room access control**. I evaluated the video approach, set up LiveKit, built the token endpoint with the participant and time window checks, and moved the chat and TTC logging onto the LiveKit room.

### Note

The AI assistant and the AI safety layer are **not yet implemented**. Week 4 focused on video and room access, and these features are planned for the coming weeks.
