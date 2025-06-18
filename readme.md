# WL1 Project Schedule - Codon Complete by July 15th

## Project Timeline

```mermaid
gantt
    title WL1 Project Timeline
    dateFormat YYYY-MM-DD
    axisFormat %m/%d
    
    section ServiceNow
    SN Delivers Student Instance          :done, sn1, 2025-06-18, 2025-06-20
    SN Delivers Instance Ready            :sn3, after k2, 7d
    
    section Kura
    Kura Defines WL Config                :done, k5, 2025-06-18, 2025-06-20
    Kura Delivers ICE Package             :k2, after sn1, 7d
    Kura Executes Workload                :k4, after sn3, 6d
    Grading Approved by Kura              :k8, after c7, 3d
    
    section Codon
    Codon Develops Grading                :c6, 2025-06-23, 2025-07-10
    Codon Grades Workload                 :c7, after k4, 2d
    
    section Timeline
    Final Prep Buffer                     :buffer, after k8, 9d
    WL1 Assignment                        :milestone, assign, 2025-07-24, 0d
```

## Key Information

**Today:** June 18, 2025 (Wednesday)

**Critical Dates:**
- June 20 (Fri): SN Instance + Kura Config complete
- June 27 (Fri): Kura ICE Package delivered  
- July 4 (Fri): SN Instance ready for workload
- July 10 (Thu): Kura workload execution + Codon development complete
- July 15 (Tue): **CODON COMPLETE** 
- July 24 (Thu): **WL1 ASSIGNMENT**

**Dependencies:**
- Kura ICE Package → SN Instance Ready → Kura Workload → Codon Grading → Kura Approval
- Codon Development runs parallel (starts June 23)
- 9-day buffer for final preparation

---
*Copy this entire content into your GitHub README.md file*
