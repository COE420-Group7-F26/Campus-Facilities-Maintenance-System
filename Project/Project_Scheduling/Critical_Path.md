Critical Path:
T1 → T3 → T4 → T5 → T7 → T8 → T9 → T10

Expected Project Duration:
34 days

Explanation:
The Critical Path was determined from the forward and backward pass calculations in Exercise 6. The tasks on the Critical Path all have Slack = 0 (ES = LS and EF = LF), which means any delay in one of them directly delays the whole project. T2 (Database Design) and T6 (Request Management Module Development) each have 1 day of slack, so they can be delayed by one day without affecting the finish date, and are therefore not critical.

Comparing all paths through the network:
- T1 → T3 → T4 → T5 → T7 → T8 → T9 → T10 = 3+5+4+6+6+3+5+2 = 34 days
- T1 → T2 → T4 → T5 → T7 → T8 → T9 → T10 = 3+4+4+6+6+3+5+2 = 33 days
- T1 → T3 → T4 → T6 → T7 → T8 → T9 → T10 = 3+5+4+5+6+3+5+2 = 33 days
- T1 → T2 → T4 → T6 → T7 → T8 → T9 → T10 = 3+4+4+5+6+3+5+2 = 32 days

The longest path is 34 days, which matches the earliest finish of T10 (EF = 34). This path is therefore the Critical Path.

Verification:
The schedule was entered into ProjectLibre using the same task durations and predecessors from the WBS. The tool calculated a total duration of 34 days and marked T1, T3, T4, T5, T7, T8, T9 and T10 as critical, which matches the manual calculations. (Screenshot below.)
