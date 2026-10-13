# Exercise 1 – Context Diagram

## Campus Facilities Maintenance System

This context diagram represents the entire Campus Facilities Maintenance System as one process.

### External Entities
- Student
- Facilities Administrator
- Maintenance Staff

### Data Flows
- Student → System: Maintenance Request Information
- System → Student: Request Status and Notifications
- Facilities Administrator → System: Request Management Information
- System → Facilities Administrator: Maintenance Request Information
- Maintenance Staff → System: Repair Updates
- System → Maintenance Staff: Assigned Request Information
