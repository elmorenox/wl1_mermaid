# WL1 Project Schedule

## Project Timeline

```mermaid
gantt
    title WL1 Project Timeline - Complete by Tuesday July 15th
    dateFormat YYYY-MM-DD
    axisFormat %m/%d
    excludes weekends
    
    section ServiceNow
    1. SN Delivers Student Instances      :sn1, 2025-06-18, 2025-06-20
    10. SN Delivers 20 Production Instances :sn10, 2025-07-02, 2025-07-04
    
    section Kura
    2. Proving Student Instance Data Method :k2, 2025-06-23, 2025-06-26
    3. Kura Creates ICE Package           :k3, 2025-06-27, 2025-07-01
    4. Kura Defines Real WL Data          :k4, 2025-07-01, 2025-07-03
    6. Kura Executes Workload             :k6, 2025-07-03, 2025-07-05
    7. Kura Defines Components/Subcomponents :k7, 2025-06-23, 2025-06-27
    
    section Codon
    8. Codon Develops Grading Logic       :c8, 2025-06-30, 2025-07-04
    11. Codon Populates 20 Instances      :c11, 2025-07-07, 2025-07-10
    9. Final Integration & Testing        :c9, 2025-07-10, 2025-07-13
```

## Project Schedule Table

| Task | Owner Org | Owner | Start Date | End Date | Duration | Status | Dependencies |
|------|-----------|-------|------------|----------|----------|--------|--------------|
| 1. SN Delivers Student Instances | ServiceNow | | Wed Jun 18 | Fri Jun 20 | 3 days | ✅ Complete | None |
| 2. Proving Student Instance Data Method | Kura | Luis | Mon Jun 23 | Thu Jun 26 | 4 days | 🔄 Ongoing | Task 1 |
| 3. Kura Creates ICE Package | Kura | Luis, Kevin | Fri Jun 27 | Tue Jul 1 | 3 days | ⏳ Pending | Task 2 |
| 7. Kura Defines Components/Subcomponents | Kura | Kevin, Luis | Mon Jun 23 | Fri Jun 27 | 5 days | 🔄 Ongoing | None |
| 10. SN Delivers 20 Production Instances | ServiceNow | | Wed Jul 2 | Fri Jul 4 | 3 days | ⏳ Pending | Task 3 |
| 4. Kura Defines Real WL Data | Kura | Luis | Wed Jul 2 | Fri Jul 4 | 3 days | ⏳ Pending | Task 3 |
| 8. Codon Develops Grading Logic | Codon | Xavier | Mon Jun 30 | Fri Jul 4 | 5 days | ⏳ Pending | Task 7 |
| 5. Codon Develops Data Population | Codon | Xavier | Mon Jul 7 | Wed Jul 9 | 3 days | ⏳ Pending | Task 4 |
| 6. Kura Executes Workload | Kura | Luis | Mon Jul 7 | Tue Jul 8 | 2 days | ⏳ Pending | Task 4 |
| 11. Codon Populate 20 Instances | Codon | Xavier | Thu Jul 10 | Fri Jul 11 | 2 days | ⏳ Pending | Task 5 |
| 9. Final Integration & Testing | Codon | Luis, Xavier | Mon Jul 14 | Tue Jul 15 | 2 days | ⏳ Pending | Tasks 11, 8, 6 |

## Detailed Task Breakdown

### Task 1: SN Delivers Student Instances
| Subtask | Description | Owner Org | Owner | Status |
|---------|-------------|-----------|-------|--------|
| 1a | ServiceNow provisions base student instances | ServiceNow |  | ✅ Complete |
| 1b | Delivery confirmation to project team | ServiceNow | | ✅ Complete |

### Task 2: Proving Student Instance Data Method
| Subtask | Description | Owner Org | Owner | Status |
|---------|-------------|-----------|-------|--------|
| 2a | Kevin creates Workload Prep Instruction | Kura | Kevin | ✅ Complete |
| 2c | Luis configures student instance to workload ready state to create data and artifacts for Codon | Kura | Luis | 🔄 Ongoing |
| 2d | URL for Student Workload Configuration Instance | Kura | Luis | ✅ Complete |
| 2e | Basic auth for Student Workload Instance | Kura | Luis | ✅ Complete |
| 2f | XML Update Set from WL Instance | Kura | Luis | ✅ Complete |
| 2g | URL for Target Student Workload Configuration Instance | Kura | Luis | ✅ Complete |
| 2h | Basic auth for Student Workload Instance | Kura | Luis | ✅ Complete |
| 2i | Codon attempts programmatic replication | Codon | Xavier | ⏳ Pending |

### Task 3: Kura Creates ICE Package
| Subtask | Description | Owner Org | Owner | Status |
|---------|-------------|-----------|-------|--------|
| 3a | IF GO: Create structure-only ICE Package | Kura | Luis, Kevin | ⏳ Pending |
| 3b | IF NO-GO: Create traditional ICE with embedded data | Kura | Luis, Kevin | ⏳ Pending |
| 3c | Delivery to ServiceNow team | Kura | Nicole | ⏳ Pending |

### Task 10: SN Delivers 20 Production Instances
| Subtask | Description | Owner Org | Owner | Status |
|---------|-------------|-----------|-------|--------|
| 10a | Install ICE Package on 20 instances | ServiceNow |  | ⏳ Pending |

### Task 4: Kura Defines Real WL Data
| Subtask | Description | Owner Org | Owner | Status |
|---------|-------------|-----------|-------|--------|
| 4a | Define actual workload data requirements | Kura | Luis | ⏳ Pending |
| 4b | Create faulty scenario specifications | Kura | Luis | ⏳ Pending |
| 4c | Document data specifications for population | Kura | Luis | ⏳ Pending |

### Task 5: Codon Develops Data Population
| Subtask | Description | Owner Org | Owner | Status |
|---------|-------------|-----------|-------|--------|
| 5a | Build production data population capability | Codon | Xavier | ⏳ Pending |
| 5b | Validate capability before production use | Codon | Luis | ⏳ Pending |

### Task 6: Kura Executes Fix
| Subtask | Description | Owner Org | Owner | Status |
|---------|-------------|-----------|-------|--------|
| 6a | Execute workload fix procedures | Kura | Luis | ⏳ Pending |
| 6b | Document expected outcomes | Kura | Luis | ⏳ Pending |

### Task 7: Kura Defines Components/Subcomponents
| Subtask | Description | Owner Org | Owner | Status |
|---------|-------------|-----------|-------|--------|
| 7a | Define WL1 grading components | Kura | Kevin, Luis | ⏳ Pending |
| 7b | Deliver specifications to Codon | Kura | Luis | ⏳ Pending |

### Task 8: Codon Develops Grading Logic
| Subtask | Description | Owner Org | Owner | Status |
|---------|-------------|-----------|-------|--------|
| 8a | Develop grading logic based on components | Codon | Xavier | ⏳ Pending |
| 8b | Build validation for each subcomponent | Codon | Xavier | ⏳ Pending |
| 8c | Test grading logic | Codon | Luis | ⏳ Pending |

### Task 11: Populate 20 Instances
| Subtask | Description | Owner Org | Owner | Status |
|---------|-------------|-----------|-------|--------|
| 11a | Use approved data population method | Codon, Students | ? | ⏳ Pending |
| 11b | Populate all 20 instances with workload data | Codon | Xavier | ⏳ Pending |
| 11c | Validate data consistency across instances | Kura | Luis | ⏳ Pending |

### Task 9: Final Integration & Testing
| Subtask | Description | Owner Org | Owner | Status |
|---------|-------------|-----------|-------|--------|
| 9a | End-to-end testing on populated instances | Codon, Kura | Luis, Xavier | ⏳ Pending |
| 9b | Final validation and sign-off | Kura | Luis | ⏳ Pending |

---
*Last Updated: June 25, 2025*
