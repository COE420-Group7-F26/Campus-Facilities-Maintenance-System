# Class Inventory / Consolidation Record

## Consolidated Class Inventory

| Class ID | Class Name | Responsibility |
|---|---|---|
| C01 | User | Stores shared user information and functionality. |
| C02 | Student | Submits maintenance requests and tracks their status. |
| C03 | Administrator | Manages requests, assigns staff, and sets priorities. |
| C04 | MaintenanceStaff | Views assigned requests and records repair activities. |
| C05 | MaintenanceRequest | Stores maintenance issue details, status, and priority. |
| C06 | RequestAssignment | Records maintenance staff assignments. |
| C07 | RequestHistory | Records changes and actions related to requests. |
| C08 | RepairRecord | Stores repair work and completion details. |
| C09 | RepairNote | Stores maintenance staff progress notes. |
| C10 | Attachment | Stores images associated with requests or repairs. |
| C11 | Notification | Stores maintenance request notifications. |
| C12 | NotificationPreference | Stores user notification preferences. |
| C13 | UserAccount | Manages account credentials and authentication. |
| C14 | Speciality | Defines maintenance staff specialities. |
| C15 | Priority | Defines maintenance request priority levels. |
| C16 | RequestStatus | Defines maintenance request statuses. |

## Consolidation and Integration Decisions

The four individual class models were consolidated into one UML Class Diagram for the Campus Facilities Maintenance System.

The User class was retained as the parent class for Student, Administrator, and MaintenanceStaff to avoid duplicating shared user information.

MaintenanceRequest was used as the central class connecting student requests, administrative assignments, repair activities, and request history.

Attachment was shared between maintenance requests and repair records to avoid unnecessary duplication.

The original request priority representation was standardized using the Priority enumeration. RequestStatus was included to represent maintenance request states consistently.

RequestAssignment connects maintenance requests with maintenance staff, while RequestHistory records request-related actions and changes.

The notification and account classes were retained to support authentication, notification delivery, and user preferences.

These decisions were reflected in the consolidated UML Class Diagram.
