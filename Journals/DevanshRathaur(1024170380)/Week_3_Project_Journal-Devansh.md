# Week 3 Project Journal — Real Time Chat Implementation & TTC Logging

## Week 3 — Real Time Chat Implementation & TTC Logging

### Project Details

| **Course** | UCS503 / UCS503P — Software Engineering |

| **Institute** | Thapar Institute of Engineering and Technology, Patiala |

| **Project** | Telemedicine Platform |

| **Member** | Devansh Rathaur 1024170380 |

| **Team Members** | Ashish Bhagat 1024170372, Devansh Rathaur 1024170380, Animesh Sudhanshu 1024170375 |

| **Project Stage** | First Iteration — Core Consultation Loop |

| **Week** | Week 3 |

### Objective for the Week

The objective of Week 3 was to implement the real time layer planned in Week 2: consultation specific chat using Socket.io, the events needed by the frontend, and the logging needed to measure time to connect.

### Day 1 — Socket.io Server Setup

Set up the Socket.io server alongside the Express backend and configured it to accept authenticated connections only.
- Defined the room naming convention based on the appointment ID, and confirmed it with the backend teammate.

### Day 2 — Consultation Rooms

Implemented joining a consultation room, with a check that the user is the booked patient or doctor of that appointment.
- Emitted join and leave events so both participants can see when the other person is present.

### Day 3 — Chat Messaging

Implemented sending and receiving messages inside a consultation room.
- Stored messages against the consultation so that the chat history can be loaded again if a participant rejoins.

### Day 4 — TTC Logging

Recorded a timestamp when each participant joins a consultation room and when both are present in the same room.
- Calculated time to connect against the scheduled start time provided by the appointment record.

### Day 5 — Connection Handling

Added reconnection handling so a dropped connection rejoins the same room and does not lose the consultation context.
- Exposed connection status events to the frontend teammate for the chat screen.

### Day 6 — Integration and Review

Tested the chat flow with the team, for example booking a slot, joining the room from both sides and exchanging messages.
- Reviewed the TTC timestamps with the backend teammate and logged remaining work: video consultation and the AI assistant.

### Week 3 Deliverables

- Socket.io server with authenticated connections.
- Consultation rooms restricted to the booked patient and doctor.
- Real time chat with stored message history.
- Join timestamps and time to connect calculation.
- Reconnection handling and connection status events for the frontend.

### Individual Contribution

My primary contribution was implementing the **real time communication layer**. I built the Socket.io server, the consultation room checks, chat messaging with stored history, the TTC logging and the reconnection handling.

### Note

The video consultation and the AI assistant are **not yet implemented**. Week 3 focused on the real time chat and TTC logging, and these features are planned for the coming weeks.
