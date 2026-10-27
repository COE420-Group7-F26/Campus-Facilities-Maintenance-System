# Class Model Consistency / Traceability Check

## Class Model Traceability

| System Functionality | Related Classes | Related Use Cases |
|---|---|---|
| Student maintenance requests | Student, MaintenanceRequest, Attachment | Submit Maintenance Request, Track Request Status |
| Administrative request management | Administrator, MaintenanceRequest, Priority | Prioritize Maintenance Request |
| Maintenance staff assignment | Administrator, RequestAssignment, MaintenanceStaff | Assign Maintenance Request |
| Request history tracking | RequestHistory, MaintenanceRequest, User | View Request History |
| Maintenance and repair operations | MaintenanceStaff, RepairRecord, RepairNote | View Assigned Requests, Update Request Status, Record Repair Completion |
| User authentication | User, UserAccount | User Login, User Logout |
| Notification management | Notification, NotificationPreference, User | Receive Status Notifications, Manage Notification Preferences |

## Consistency Verification

### 1. Requirements and Use Cases
The consolidated model represents the main system functions identified in previous labs, including submitting requests, tracking status, assigning staff, recording repairs, and notifying users.

### 2. Data Flow Diagram Consistency
MaintenanceRequest, RequestAssignment, RequestHistory, RepairRecord, and Notification represent information handled by the system's major processes, including request management, assignments, repairs, and notifications.

### 3. Relationships and Multiplicities
A student can submit multiple maintenance requests, while each request belongs to one student.

Maintenance requests are associated with assignments, history records, and attachments.

Maintenance staff members can receive assigned requests and record repair activities.

User provides inheritance relationships for Student, Administrator, and MaintenanceStaff.

### 4. Overall Model Consistency
The consolidated UML Class Diagram combines the individual models into one representation of the Campus Facilities Maintenance System.

It includes the main classes, attributes, methods, associations, multiplicities, and inheritance relationships required to represent the proposed system.
