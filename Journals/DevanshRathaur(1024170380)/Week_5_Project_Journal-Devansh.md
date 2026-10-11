# Week 5 Project Journal — AI Pre-Consultation Assistant & Safety Layer

## Week 5 — AI Pre-Consultation Assistant & Safety Layer

### Project Details

| **Course** | UCS503 / UCS503P — Software Engineering |

| **Institute** | Thapar Institute of Engineering and Technology, Patiala |

| **Project** | Telemedicine Platform |

| **Member** | Devansh Rathaur 1024170380 |

| **Team Members** | Ashish Bhagat 1024170372, Devansh Rathaur 1024170380, Animesh Sudhanshu 1024170375 |

| **Project Stage** | Second Iteration — AI Assistant, Records and Hardening |

| **Week** | Week 5 |

### Objective for the Week

The objective of Week 5 was to implement the Gemini based pre consultation assistant planned in Week 2, together with its emergency safety layer, usage quota and tests.

### Day 1 — Gemini Integration

Integrated the Gemini API for conversational symptom intake, with replies streamed to the frontend.
- Wrote the system instructions so that the assistant only prepares context for the doctor and never diagnoses or prescribes.

### Day 2 — Triage Tools and Emergency Override

Defined the triage tools the assistant can call to record symptoms in a structured form.
- Added the emergency override, so that symptoms such as chest pain, stroke signs or self harm always produce a seek immediate care response instead of normal advice.

### Day 3 — Usage Quota and Conversation Storage

Added an hourly usage quota per patient and checked it before every assistant request.
- Stored conversations so that a patient can continue a chat and the doctor can see the prepared summary.

### Day 4 — Medical History Search

Added search over the patient's own records and profile, so the assistant can use their history when answering.
- Restricted the search to the logged in patient's data only, and made the assistant continue without it if the search fails.

### Day 5 — AI Safety Regression Suite

Wrote a fixed set of symptom prompts, including emergency cases, that must all be routed to the seek immediate care response.
- Added the suite to the CI pipeline so that it runs before each release.

### Day 6 — Integration and Review

Tested the assistant with the team using normal and emergency symptoms, and checked the quota and the saved summary.
- Reviewed the safety rules and logged remaining work: final end to end testing and the pilot.

### Week 5 Deliverables

- Gemini based symptom intake assistant with streamed replies.
- Triage tools and emergency override.
- Hourly quota and stored conversations.
- Patient scoped medical history search with graceful fallback.
- AI safety regression suite running in CI.

### Individual Contribution

My primary contribution was implementing the **AI pre consultation assistant and its safety layer**. I built the Gemini integration, the triage tools and emergency override, the quota, the patient scoped history search and the regression suite for AI safety.

### Note

The pilot with test users and the final end to end testing are **not yet done**. Week 5 focused on the AI assistant and its safety layer, and these remaining items are planned for the coming weeks.
