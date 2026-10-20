# Exercise 1 – Shahad Alshamsi (g00100329) – Maintenance Staff & Repairs

| Class ID | Class Name | Purpose/Responsibility | Related Use Case(s) | Contributor |
|---|---|---|---|---|
| C09 | MaintenanceStaff | Represents a maintenance worker who receives assigned requests, updates their status, adds repair notes, and records completion. Inherits shared account information from User. | View Assigned Requests (UC-18), Update Request Status, Record Repair Completion (UC-20) | Shahad Alshamsi |
| C10 | RepairRecord | Stores the repair work done for one maintenance request: start date, completion date, work description, materials used, and completion photos. | Record Repair Completion (UC-20), Update Request Status | Shahad Alshamsi |
| C11 | RepairNote | Stores progress notes written by the staff member while working on a repair, so the administrator and student can follow what was done. | Add Repair Notes, Update Request Status | Shahad Alshamsi |
| C12 | Specialty (enumeration) | Defines the fixed list of staff specialties (Electrical, Plumbing, Air Conditioning, Furniture, Cleaning, General) so requests can be matched to the right staff member. | View Assigned Requests (UC-18), Assign Maintenance Request | Shahad Alshamsi |
