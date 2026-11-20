# Lab 9 — Function Point Analysis
**Mohammad Shayan Kafeel — b00097076**

## Task 4: Calculate Function Points

The final Adjusted Function Points (FP) are calculated using the Unadjusted Function Points (UFP) from Task 2 and the Value Adjustment Factor (VAF) from Task 3.

| Description | Value |
|---|---:|
| Unadjusted Function Points (UFP) | 139 |
| Total Degree of Influence (TDI) | 41 |
| Value Adjustment Factor (VAF) | 1.06 |
| Final Adjusted Function Points (FP) | **147.34** |

### Calculation
FP = UFP × VAF  
FP = 139 × 1.06  
**FP = 147.34 Function Points**

### Interpretation
The final result is 147.34 Function Points. This represents the estimated functional size of our Campus Facilities Maintenance System after considering its general system characteristics.

The adjusted value is slightly higher than the UFP because the system includes online data entry, maintenance request updates, performance requirements, and notification features.

## Task 5: Software Effort and Cost Estimation

Using the final Function Points calculated in Task 4, we estimated the development effort, personnel cost, working hours, and project duration.

### Given Assumptions

| Assumption | Value |
|---|---|
| Final Function Points (FP) | 147.34 |
| Productivity Rate | 10 FP per Person-Month |
| Cost per Person-Month | USD 5,000 |
| Working Hours per Person-Month | 160 hours |
| Development Team Size | 4 full-time developers |

### 1. Estimate Development Effort
Effort (PM) = FP / Productivity Rate  
Effort = 147.34 / 10  
**Effort = 14.734 Person-Months**

### 2. Estimate Development Cost
Estimated Cost = Effort (PM) × Cost per PM  
Estimated Cost = 14.734 × 5,000  
**Estimated Cost = USD 73,670**

### 3. Estimate Development Hours
Estimated Hours = Effort (PM) × 160  
Estimated Hours = 14.734 × 160  
**Estimated Hours = 2,357.44 hours**

### 4. Estimate Project Duration
Duration (Months) = Effort (PM) / 4  
Duration = 14.734 / 4  
**Estimated Duration = 3.68 months**

### 5. Interpretation of Results

| Estimation | Final Result |
|---|---|
| Adjusted Function Points | 147.34 FP |
| Development Effort | 14.734 Person-Months |
| Personnel Cost | USD 73,670 |
| Development Hours | 2,357.44 hours |
| Project Duration | 3.68 months |

Based on our calculations, the Campus Facilities Maintenance System has an estimated functional size of 147.34 Function Points.

With four full-time developers, the project would take approximately 3.68 months to complete, with an estimated personnel cost of USD 73,670.

These estimates assume a productivity rate of 10 Function Points per Person-Month and 160 working hours per month.

The actual time and cost may differ depending on the team's experience, technical difficulties, and changes in requirements. The cost also covers personnel only and does not include software licenses, hardware, hosting, or other operational expenses.
