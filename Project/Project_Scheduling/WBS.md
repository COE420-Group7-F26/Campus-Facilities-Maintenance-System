# Exercise 4: Work Breakdown Structure (WBS)

| ID | Task Name | Description | Predecessor(s) | Duration (Days) |
|---|---|---|---|---|
| T1 | Requirements Refinement | Review and finalize the functional and non-functional requirements of the system. | — | 3 |
| T2 | Database Design | Design the database for users, maintenance requests, assignments, and repair records. | T1 | 4 |
| T3 | User Interface Design | Design the web pages for students, facilities administrators, and maintenance staff. | T1 | 5 |
| T4 | User Authentication Development | Implement login and role-based access for the three user types. | T2, T3 | 4 |
| T5 | Maintenance Request Module Development | Develop request submission, viewing, tracking, and photo attachment features. | T4 | 6 |
| T6 | Request Management Module Development | Develop request review, prioritization, assignment, and reassignment features. | T4 | 5 |
| T7 | Repair and Notification Module Development | Develop repair status updates, repair notes, completion records, and notifications. | T5, T6 | 6 |
| T8 | System Integration | Integrate all modules and verify that they work together. | T7 | 3 |
| T9 | System Testing | Test functionality, security, and performance, and fix identified issues. | T8 | 5 |
| T10 | Deployment Preparation | Prepare the completed web system for deployment and final review. | T9 | 2 |
