# WL1 Project Schedule

## Project Timeline

```mermaid
gantt
    title WL1 Project Timeline - Complete by Friday July 4th
    dateFormat YYYY-MM-DD
    axisFormat %m/%d
    
    section ServiceNow
    1. SN Delivers Student Instances      :sn1, 2025-06-18, 2025-06-20
    10. SN Delivers 20 Production Instances :sn10, after k2, 2d
    11. Populate 20 Instances             :sn11, after c5, 1d
    
    section Kura
    3. Proving the Method                 :k3, 2025-06-23, 2025-06-24
    2. Kura Creates ICE Package           :k2, after k3, 2d
    4. Kura Defines Real WL Data          :k4, after k2, 2d
    6. Kura Executes Fix                  :k6, after k4, 2d
    7. Kura Defines Components/Subcomponents :k7, 2025-06-23, 2025-06-26
    
    section Codon
    5. Codon Develops Data Population     :c5, after k4, 2d
    8. Codon Develops Grading Logic       :c8, after k7, 3d
    9. Final Integration & Testing        :c9, after sn11 c8 k6, 1d
```

## Project Schedule Table

| Task | Owner Org | Owner | Start Date | End Date | Duration | Status | Dependencies |
|------|-----------|-------|------------|----------|----------|--------|--------------|
| 1. SN Delivers Student Instances | ServiceNow | | Wed Jun 18 | Fri Jun 20 | 3 days | ✅ Complete | None |
| 3. Proving the Method | Kura | Luis | Mon Jun 23 | Tue Jun 24 | 2 days | ⏳ Pending | Task 1 |
| 2. Kura Creates ICE Package | Kura | Luis, Kevin | Wed Jun 25 | Thu Jun 26 | 2 days | ⏳ Pending | Task 3 |
| 7. Kura Defines Components/Subcomponents | Kura | Kevin, Luis | Mon Jun 23 | Thu Jun 26 | 4 days | ⏳ Pending | None |
| 10. SN Delivers 20 Production Instances | ServiceNow | | Fri Jun 27 | Mon Jun 30 | 2 days | ⏳ Pending | Task 2 |
| 4. Kura Defines Real WL Data | Kura | Luis | Fri Jun 27 | Mon Jun 30 | 2 days | ⏳ Pending | Task 2 |
| 8. Codon Develops Grading Logic | Codon | Xavier | Fri Jun 27 | Tue Jul 1 | 3 days | ⏳ Pending | Task 7 |
| 5. Codon Develops Data Population | Codon | Xavier | Tue Jul 1 | Wed Jul 2 | 2 days | ⏳ Pending | Task 4 |
| 6. Kura Executes Fix | Kura | Luis | Tue Jul 1 | Wed Jul 2 | 2 days | ⏳ Pending | Task 4 |
| 11. Populate 20 Instances | Codon | Xavier | Thu Jul 3 | Thu Jul 3 | 1 day | ⏳ Pending | Task 5 |
| 9. Final Integration & Testing | Codon | Luis, Xavier | Fri Jul 4 | Fri Jul 4 | 1 day | ⏳ Pending | Tasks 11, 8, 6 |

## Detailed Task Breakdown

### Task 1: SN Delivers Student Instances
| Subtask | Description | Owner Org | Owner | Status |
|---------|-------------|-----------|-------|--------|
| 1a | ServiceNow provisions base student instances | ServiceNow |  | ✅ Complete |
| 1b | Delivery confirmation to project team | ServiceNow | | ✅ Complete |

### Task 3: Proving the Method
| Subtask | Description | Owner Org | Owner | Status |
|---------|-------------|-----------|-------|--------|
| 3a | Kura manually creates faulty flow with test data | Kura | Luis | ⏳ Pending |
| 3b | Document exactly what was created manually | Kura | Luis | ⏳ Pending |
| 3c | Communicate requirements to Codon | Kura | Luis | ⏳ Pending |
| 3d | Codon attempts programmatic replication | Codon | Xavier | ⏳ Pending |
| 3e | Validate method success/failure | Kura | Luis | ⏳ Pending |
| 3f | **GO/NO-GO DECISION** | Kura | Luis | ⏳ Pending |

### Task 2: Kura Creates ICE Package
| Subtask | Description | Owner Org | Owner | Status |
|---------|-------------|-----------|-------|--------|
| 2a | IF GO: Create structure-only ICE Package | Kura | Luis, Kevin | ⏳ Pending |
| 2b | IF NO-GO: Create traditional ICE with embedded data | Kura | Luis, Kevin | ⏳ Pending |
| 2c | Delivery to ServiceNow team | Kura | Nicole | ⏳ Pending |

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
*Last Updated: June 20, 2025*
