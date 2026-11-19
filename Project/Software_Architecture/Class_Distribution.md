# Lab 8 - Exercise 3: Class Distribution

Project: Campus Facilities Maintenance System
Contributor: Shahad Alshamsi (g00100329)

All 16 classes from the consolidated Lab 5 UML Class Diagram are assigned to exactly one primary component.

| ID | Component Name | Layer | Responsibilities | Included Classes |
|---|---|---|---|---|
| CO1 | User Interface | Presentation | Displays screens for students, administrators, and maintenance staff; collects input and shows results. | — (UI screens only) |
| CO2 | User & Account Management | Business Logic | Manages user information, authentication, account credentials, and role-specific user operations. | User, Student, Administrator, MaintenanceStaff, UserAccount |
| CO3 | Request Management | Business Logic | Creates and stores maintenance requests, assigns them to staff, records request history, and stores issue photos. | MaintenanceRequest, RequestAssignment, RequestHistory, Attachment, Specialty, Priority, RequestStatus |
| CO4 | Repair Management | Business Logic | Records repair work, progress notes, and repair completion details. | RepairRecord, RepairNote |
| CO5 | Notification Management | Business Logic | Creates and delivers status-change notifications and manages user notification preferences. | Notification, NotificationPreference |
| CO6 | Data Access | Data Access | Stores and retrieves all system data and logs application errors. | — (data-access logic only) |

## Class Coverage Check

| Class ID | Class Name | Assigned Component |
|---|---|---|
| C01 | User | CO2 – User & Account Management |
| C02 | Student | CO2 – User & Account Management |
| C03 | Administrator | CO2 – User & Account Management |
| C04 | MaintenanceStaff | CO2 – User & Account Management |
| C05 | MaintenanceRequest | CO3 – Request Management |
| C06 | RequestAssignment | CO3 – Request Management |
| C07 | RequestHistory | CO3 – Request Management |
| C08 | RepairRecord | CO4 – Repair Management |
| C09 | RepairNote | CO4 – Repair Management |
| C10 | Attachment | CO3 – Request Management |
| C11 | Notification | CO5 – Notification Management |
| C12 | NotificationPreference | CO5 – Notification Management |
| C13 | UserAccount | CO2 – User & Account Management |
| C14 | Specialty | CO3 – Request Management |
| C15 | Priority | CO3 – Request Management |
| C16 | RequestStatus | CO3 – Request Management |

**Result:** 16 of 16 classes assigned; no class is assigned to more than one component.

## Distribution Decisions

- **User subclasses stay together.** Student, Administrator, and MaintenanceStaff inherit from User, so they are kept in the same component as User and UserAccount to avoid splitting an inheritance hierarchy.
- **RequestAssignment is in Request Management.** An assignment links one maintenance request to one staff member and is created when a request is assigned, so it belongs with the request it describes.
- **Attachment is in Request Management.** Attachments are shared by maintenance requests (issue photos) and repair records (completion photos). Request Management is its primary component; Repair Management uses it through Request Management's interface.
- **Enumerations follow the class that uses them most.** Priority, RequestStatus, and Specialty are attributes of MaintenanceRequest (priority, status, category), so they are placed in Request Management. MaintenanceStaff also uses Specialty through that component.
- **Repair classes are separate from request classes.** RepairRecord and RepairNote describe the repair work, not the request itself, which matches the separation used in the Lab 5 Class Diagram and the Lab 6/7 UC-20 diagrams.
- **CO1 and CO6 have no Lab 5 classes.** The Lab 5 Class Diagram models domain classes only, so the Presentation and Data Access layers contain interface and data-access logic rather than domain classes.
