# Lab 9 - Task 3: Value Adjustment Factor (VAF)

Project: Campus Facilities Maintenance System
Student: Shahad Alshamsi – g00100329

The 14 General System Characteristics (GSCs) were evaluated based on the requirements of the Campus Facilities Maintenance System. Each characteristic was assigned a Degree of Influence (Fi) from 0 to 5.

| No. | General System Characteristic | Fi | Justification |
|---|---|---:|---|
| 1 | Data Communications | 3 | Students, administrators, and maintenance staff exchange information through the online system. |
| 2 | Distributed Data Processing | 1 | The system uses layered architecture, but distributed processing is not specifically required. |
| 3 | Performance | 4 | The system must load pages and retrieve maintenance requests quickly. |
| 4 | Heavily Used Configuration | 2 | The system supports multiple users without special hardware requirements. |
| 5 | Transaction Rate | 3 | Students submit requests, while administrators and staff regularly update them. |
| 6 | Online Data Entry | 5 | Users enter maintenance requests, assignments, repair notes, and status updates online. |
| 7 | End-User Efficiency | 4 | The system provides simple request submission and clear validation messages. |
| 8 | Online Update | 5 | Requests, priorities, assignments, and repair records can be updated online. |
| 9 | Complex Processing | 2 | The system checks duplicate requests and manages status changes. |
| 10 | Reusability | 2 | The layered architecture separates functions into reusable components. |
| 11 | Installation Ease | 1 | Users access the system through supported web browsers. |
| 12 | Operational Ease | 3 | Notifications, automatic logout, error logs, and backups support operations. |
| 13 | Multiple Sites | 2 | The system handles different campus locations, but multiple deployment sites are not required. |
| 14 | Facilitate Change | 4 | Administrators can update categories and locations without modifying the source code. |
| | **Total Degree of Influence (TDI)** | **41** | |

### VAF Calculation

**TDI = Σ Fi = 41**

VAF = 0.65 + (0.01 × TDI)

VAF = 0.65 + (0.01 × 41)

VAF = 0.65 + 0.41

**VAF = 1.06**

### Interpretation

The Value Adjustment Factor is 1.06, meaning the system's general characteristics increase its unadjusted functional size by 6%. This reflects the system's online operations, performance requirements, and ability to handle maintenance requests and updates efficiently.
