# WL1 Project Schedule 

## Project Timeline

```mermaid
gantt
    title WL1 Project Timeline
    dateFormat YYYY-MM-DD
    axisFormat %m/%d
    
    section ServiceNow
    1. SN Delivers Student Instance       :sn1, 2025-06-18, 2025-06-20
    3. SN Delivers Instance Ready         :sn3, after k2, 7d
    
    section Kura
    5. Kura Defines WL Config             :k5, 2025-06-18, 2025-06-20
    2. Kura Delivers ICE Package          :k2, after sn1, 7d
    4. Kura Executes Workload             :k4, after sn3, 6d
    8. Grading Approved by Kura           :k8, after c7, 3d
    
    section Codon
    6. Codon Develops Grading             :c6, 2025-06-23, 2025-07-10
    7. Codon Grades Workload              :c7, after k4, 2d
```

## Project Schedule Table

| Task | Owner Org | Owner | Start Date | End Date | Duration | Status | Dependencies |
|------|-----------|-------|------------|----------|----------|--------|--------------|
| 1. SN Delivers Student Instance | ServiceNow | [Name] | Wed Jun 18 | Fri Jun 20 | 3 days | ✅ Complete | None |
| 2. Kura Delivers ICE Package to SN | Kura | [Name] | Fri Jun 20 | Fri Jun 27 | 7 days | 🔄 In Progress | Task 1 |
| 3. SN Delivers Student Instance Ready | ServiceNow | [Name] | Fri Jun 27 | Fri Jul 4 | 7 days | ⏳ Pending | Task 2 |
| 4. Kura Executes Workload | Kura | [Name] | Fri Jul 4 | Thu Jul 10 | 6 days | ⏳ Pending | Task 3 |
| 5. Kura Defines WL Config | Kura | [Name] | Wed Jun 18 | Fri Jun 20 | 3 days | ✅ Complete | None |
| 6. Codon Develops Grading Capability | Codon | [Name] | Mon Jun 23 | Thu Jul 10 | 18 days | ⏳ Pending | Tasks 4, 5 |
| 7. Codon Grades Workload | Codon | [Name] | Thu Jul 10 | Sat Jul 12 | 2 days | ⏳ Pending | Task 6 |
| 8. Grading Approved by Kura | Kura | [Name] | Sat Jul 12 | Tue Jul 15 | 3 days | ⏳ Pending | Task 7 |

## Detailed Task Breakdown

### Task 1: SN Delivers Student Instance
| Subtask | Description | Owner Org | Owner | Status |
|---------|-------------|-----------|-------|--------|
| 1a | ServiceNow provisions base student instance | ServiceNow | [Name] | ✅ Complete |
| 1b | Basic instance configuration and setup | ServiceNow | [Name] | ✅ Complete |
| 1c | Delivery confirmation to project team | ServiceNow | [Name] | ⏳ Pending  |



### Task 2: Kura Delivers ICE Package to SN
| Subtask | Description | Owner Org | Owner | Status |
|---------|-------------|-----------|-------|--------|
| 2a | Prepare ICE Package| Kura | [Name] | 🔄 In Progress |
| 2b | Package validation and testing | Kura | [Name] | ⏳ Pending |
| 2c | Delivery to ServiceNow team | Kura | [Name] | ⏳ Pending |
| 2d | Installation instructions and documentation | Kura | [Name] | ⏳ Pending |


### Task 3: SN Delivers Student Instance Ready for Workload Execution
| Subtask | Description | Owner Org | Owner | Status |
|---------|-------------|-----------|-------|--------|
| 3a | Configure instance for workload execution | ServiceNow | [Name] | ⏳ Pending |
| 3b | Create Update Set | ServiceNow | [Name] | ⏳ Pending |
| 3c | Create Workflow with SLA breach, incident row, faulty notification | ServiceNow | [Name] | ⏳ Pending |
| 3d | Instance validation and testing | ServiceNow | [Name] | ⏳ Pending |

### Task 4: Kura Executes Workload
| Subtask | Description | Owner Org | Owner | Status |
|---------|-------------|-----------|-------|--------|
| 4a | Fix notification step in workflow | Kura | [Name] | ⏳ Pending |
| 4b | New notification in workflow | Kura | [Name] | ⏳ Pending |
| 4c | New incident in incidents table | Kura | [Name] | ⏳ Pending |
| 4d | Validate workload completion | Kura | [Name] | ⏳ Pending |

### Task 5: Kura Defines WL Config
| Subtask | Description | Owner Org | Owner | Status |
|---------|-------------|-----------|-------|--------|
| 5a | WL Configuration delivered EOD June 20th | Kura | [Name] | ✅ Complete |
| 5b | Define WL1 Components: WIP, Notification, Workflow, Scripting | Kura | [Name] | ✅ Complete |

### Task 6: Codon Develops Grading Capability
| Subtask | Description | Owner Org | Owner | Status |
|---------|-------------|-----------|-------|--------|
| 6a | Development starts June 23rd | Codon | [Name] | ⏳ Pending |
| 6b | Develop query logic via Records API | Codon | [Name] | ⏳ Pending |
| 6c | Build count validation and incident-notification relationship checks | Codon | [Name] | ⏳ Pending |
| 6d | TBD: Additional grading requirements | Codon | [Name] | ⏳ Pending |

### Task 7: Codon Grades Workload
| Subtask | Description | Owner Org | Owner | Status |
|---------|-------------|-----------|-------|--------|
| 7a | Execute grading against student instance | Codon | [Name] | ⏳ Pending |
| 7b | Generate grading results | Codon | [Name] | ⏳ Pending |
| 7c | Validate grading accuracy | Codon | [Name] | ⏳ Pending |

### Task 8: Grading Approved by Kura
| Subtask | Description | Owner Org | Owner | Status |
|---------|-------------|-----------|-------|--------|
| 8a | Kura validates grading logic and results | Kura | [Name] | ⏳ Pending |
| 8b | Final approval for WL1 launch | Kura | [Name] | ⏳ Pending |
| 8c | Sign-off for production deployment | Kura | [Name] | ⏳ Pending |

---
*Last Updated: June 20, 2025*
