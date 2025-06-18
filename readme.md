# WL1 Project Schedule - Codon Complete by July 15th

## Project Timeline

```mermaid
gantt
    title WL1 Project Timeline
    dateFormat YYYY-MM-DD
    axisFormat %m/%d
    
    section ServiceNow
    SN Delivers Student Instance          :sn1, 2025-06-18, 2025-06-20
    SN Delivers Instance Ready            :sn3, after k2, 7d
    
    section Kura
    Kura Defines WL Config                :k5, 2025-06-18, 2025-06-20
    Kura Delivers ICE Package             :k2, after sn1, 7d
    Kura Executes Workload                :k4, after sn3, 6d
    Grading Approved by Kura              :k8, after c7, 3d
    
    section Codon
    Codon Develops Grading                :c6, 2025-06-23, 2025-07-10
    Codon Grades Workload                 :c7, after k4, 2d
```
