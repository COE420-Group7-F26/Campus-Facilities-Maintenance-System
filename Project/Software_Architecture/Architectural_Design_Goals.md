# Lab 8 - Exercise 1: Architectural Design Goals

Project: Campus Facilities Maintenance System
Contributor: Maryam Almheiri

The following architectural design goals were selected based on the non-functional requirements identified in Lab 3.

| Goal ID | Design Goal | Description | Related Requirement | Priority | Justification |
|---|---|---|---|---|---|
| DG-01 | Security | Ensure that only authorized users can access the system and its functions. | NFR-02: Users must log in before accessing system functions. | High | The system contains student information and maintenance requests, so access must be protected. |
| DG-02 | Performance | Ensure that the system processes maintenance requests quickly and efficiently. | NFR-06: Maintenance request submissions must be processed within 2 seconds under normal conditions. | High | Students need to submit requests without unnecessary delays, especially when reporting urgent maintenance issues. |
| DG-03 | Maintainability | Make the system easier to maintain, troubleshoot, and update. | NFR-10: Application errors must be logged with their date and time. | Medium | Keeping error records helps developers identify problems and fix them more easily. |

## Conclusion

These goals focus on keeping the Campus Facilities Maintenance System secure, responsive, and easy to maintain. They will help guide the selection of an appropriate architectural style and the design of the system's components in the following exercises.
