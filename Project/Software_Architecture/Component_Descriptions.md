# Lab 8 - Exercise 3: Component Descriptions

Project: Campus Facilities Maintenance System
Contributor: Shahad Alshamsi (g00100329)

The components below follow the **Layered Architecture** selected in Exercise 2. The system is divided into **six components** across the three software layers:

| Layer | Components |
|---|---|
| Presentation Layer | CO1 – User Interface |
| Business Logic Layer | CO2 – User & Account Management, CO3 – Request Management, CO4 – Repair Management, CO5 – Notification Management |
| Data Access Layer | CO6 – Data Access |

Each layer only uses the layer directly below it: the User Interface calls the business components, and the business components read and write data only through the Data Access component.

---

## CO1 – User Interface (Presentation Layer)

**Responsibilities**
- Display the screens used by students, facilities administrators, and maintenance staff.
- Collect user input (login details, request details, photos, repair updates) and pass it to the business components.
- Show results returned by the business components, such as request status, assigned requests, and notifications.

**Supported functionality:** all use cases, since every actor interacts with the system through this component.

**Included classes:** none. This component contains user-interface screens only, not domain classes from Lab 5.

---

## CO2 – User & Account Management (Business Logic Layer)

**Responsibilities**
- Store and manage shared user information for all user types.
- Authenticate users and manage account credentials and account status.
- Provide the role-specific operations of students, administrators, and maintenance staff.

**Supported functionality:** User Login, account deactivation, role-based access for Student, Facilities Administrator, and Maintenance Staff. Supports design goal **DG-01 Security** (NFR-02: users must log in before accessing system functions).

**Included classes:** User, Student, Administrator, MaintenanceStaff, UserAccount

---

## CO3 – Request Management (Business Logic Layer)

**Responsibilities**
- Create and store maintenance requests with their location, description, category, priority, and status.
- Assign and reassign requests to suitable maintenance staff.
- Record the history of actions performed on each request.
- Store photos attached to requests.

**Supported functionality:** Submit Maintenance Request (UC-01), Select Issue Category, Attach Issue Photo, Prioritize Maintenance Request, Assign Maintenance Request (UC-04), Reassign Maintenance Request, View Request Status, View/Search/Filter Maintenance Requests, View Request History, Cancel Maintenance Request. Supports design goal **DG-02 Performance** (NFR-06: request submission within 2 seconds).

**Included classes:** MaintenanceRequest, RequestAssignment, RequestHistory, Attachment, Specialty, Priority, RequestStatus

---

## CO4 – Repair Management (Business Logic Layer)

**Responsibilities**
- Record the repair work performed for each maintenance request.
- Store repair start and completion dates, work descriptions, and materials used.
- Store progress notes written by maintenance staff during a repair.
- Mark repairs as completed and calculate repair duration.

**Supported functionality:** View Assigned Requests (UC-18), Add Repair Notes, Update Request Status, Upload Completion Photo, Record Repair Completion (UC-20, FR-20).

**Included classes:** RepairRecord, RepairNote

---

## CO5 – Notification Management (Business Logic Layer)

**Responsibilities**
- Create notifications when the status of a maintenance request changes.
- Deliver notifications to users and track whether they have been read.
- Store and apply each user's notification preferences.

**Supported functionality:** Receive Status Notification (UC-09), notification preference settings.

**Included classes:** Notification, NotificationPreference

---

## CO6 – Data Access (Data Access Layer)

**Responsibilities**
- Save, retrieve, update, and delete system data (users, requests, assignments, repair records, notifications) in the database.
- Hide database details from the business components so that the database can change without affecting business logic.
- Log application errors with their date and time.

**Supported functionality:** persistence for all business components. Supports design goal **DG-03 Maintainability** (NFR-10: application errors logged with date and time) and **DG-01 Security**, since no other component accesses the database directly.

**Included classes:** none. This component contains data-access (repository) logic, not domain classes from Lab 5.
