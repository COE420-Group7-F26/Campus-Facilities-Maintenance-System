# Exercise 2 – Select and Justify an Architectural Style

**Contributor:** Maryam Alteneiji  
**Selected Architectural Style:** Layered Architecture

## Main Characteristics

The Campus Facilities Maintenance System will use a Layered Architecture. The system is organized into separate layers, where each layer has a specific responsibility:

1. Presentation Layer – handles interaction with students, administrators, and maintenance staff.
2. Business Logic Layer – handles maintenance request processing, request assignment, status updates, and notifications.
3. Data Access Layer – manages communication between the business logic and stored data.
4. Database Layer – stores users, maintenance requests, assignments, repair records, and related information.

## Why It Is Appropriate

Layered Architecture is suitable for the Campus Facilities Maintenance System because it separates the different responsibilities of the system. The user interface does not directly access or modify stored data. Instead, requests are processed through the business logic and data access layers. This makes the system easier to understand, maintain, and update.

## Support for Design Goals

### Security
The layered structure supports security by controlling access to system data. Users interact with the system through the appropriate layers instead of accessing the database directly.

### Performance
The separation of responsibilities allows business operations and data access to be improved independently, helping the system process maintenance requests efficiently.

### Maintainability
Changes can be made to one layer with limited impact on the other layers. This makes it easier to troubleshoot, maintain, and extend the system.

## Advantages

- Clear separation of responsibilities.
- Easier maintenance and testing.
- Better organization of the system.
- Controlled access to system data.
- Easier to modify or extend individual parts of the system.

## Potential Limitations

Layered Architecture may introduce additional communication between layers, which can add some processing overhead. It can also become unnecessarily complex if too many layers are created. For this project, using only the necessary layers will help keep the architecture simple and manageable.
