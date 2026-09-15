# Risk Register

**Project:** Campus Facilities Maintenance System
**Course:** COE420L – Software Engineering, Lab 2
**Prepared by:** Shahad Alshamsi – g00100329

---

| Risk ID | Risk Description | Possible Cause | Probability | Impact | Mitigation / Response Strategy |
|---|---|---|---|---|---|
| R1 | The requirements might shift or stay vague as we build the system. | Students, maintenance staff, and administrators each view the request process differently, so what one group expects from submission, assignment, or tracking might not match another. | Medium | High | We will agree on the core requirements at the start and revisit them together as a team. If something changes later, we will adjust the system in steps and finish the highest-priority features first. |
| R2 | Certain features may turn out to be hard to build or connect. | Login, request tracking, status updates, database storage, and notifications all depend on one another to function properly. | Medium | High | We will break the system into smaller pieces and test each one on its own before connecting it to the rest. We will also look into any technical obstacles early rather than leaving them until the end. |
| R3 | A team member may not be free to work on the project when needed. | Exams, assignments from other courses, and personal commitments come up during the semester. | Medium | Medium | We will split the work clearly, set our own internal deadlines, and stay in regular contact so someone else can step in if a member becomes unavailable. |
| R4 | The project could slip behind schedule. | Coding, debugging, testing, and putting the different parts together often take more time than planned. | Medium | High | We will lay out a straightforward schedule with a deadline for every increment and begin the larger features early. We will review our progress often and shift tasks around if we notice we are falling behind. |
| R5 | User details or maintenance request data might end up visible to people who should not see it. | Weak login security, incorrect permissions, or careless handling of stored user and request data. | Low | High | We will require authentication and assign different permission levels so each user only sees what they are meant to. We will also validate inputs and avoid keeping sensitive information we do not need. |

---

## Notes

- Probability and impact are assessed on a three-point scale (Low / Medium / High).
- Risks will be reviewed at the start of each increment and updated as the project progresses.
