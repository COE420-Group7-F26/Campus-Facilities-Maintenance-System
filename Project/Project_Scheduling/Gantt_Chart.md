# Exercise 5 — Gantt Chart

**Project:** Campus Facilities Maintenance System  
**Based on:** Exercise 4 — Work Breakdown Structure (`WBS.md`)  
**Schedule convention:** Day 0 is the project start. Task intervals are start-inclusive and finish-exclusive; for example, T1 runs from Day 0 to Day 3 (3 days). All dependencies are finish-to-start with no added lag.

![Gantt Chart](Gantt_Chart.png)

| ID | Task | Duration (days) | Predecessor(s) | Start day | Finish day |
|---|---|---:|---|---:|---:|
| T1 | Requirements Refinement | 3 | — | 0 | 3 |
| T2 | Database Design | 4 | T1 | 3 | 7 |
| T3 | User Interface Design | 5 | T1 | 3 | 8 |
| T4 | User Authentication Development | 4 | T2, T3 | 8 | 12 |
| T5 | Maintenance Request Module Development | 6 | T4 | 12 | 18 |
| T6 | Request Management Module Development | 5 | T4 | 12 | 17 |
| T7 | Repair and Notification Module Development | 6 | T5, T6 | 18 | 24 |
| T8 | System Integration | 3 | T7 | 24 | 27 |
| T9 | System Testing | 5 | T8 | 27 | 32 |
| T10 | Deployment Preparation | 2 | T9 | 32 | 34 |

**Planned project duration:** 34 days (Day 0 through Day 34).

**Scheduling explanation:** T2 and T3 run in parallel after T1; T4 waits for both. T5 and T6 run in parallel after T4; T7 waits for both. T8, T9 and T10 then run sequentially. This schedule uses the exact task durations and predecessors from the group's Exercise 4 WBS.

**Note:** These are relative project days, not calendar dates; no project start date was specified in the WBS.
