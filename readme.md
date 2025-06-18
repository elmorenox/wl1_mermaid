# WL1 Project Schedule - Codon Complete by July 15th

## Project Timeline

```mermaid
gantt
    title WL1 Project Timeline - Assignment July 24th
    dateFormat YYYY-MM-DD
    axisFormat %m/%d
    
    section SN Tasks
    SN-1: Student Instance (Jun 18-20)          :done, sn1, 2025-06-18, 2025-06-20
    SN-3: Instance Ready (Jun 27-Jul 4)         :sn3, after k2, 7d
    
    section K Tasks  
    K-5: WL Config (Jun 18-20)                  :done, k5, 2025-06-18, 2025-06-20
    K-2: ICE Package (Jun 20-27)                :k2, after sn1, 7d
    K-4: Execute Workload (Jul 4-10)            :k4, after sn3, 6d
    K-8: Grading Approval (Jul 12-15)           :k8, after c7, 3d
    
    section C Tasks
    C-6: Develop Grading (Jun 23-Jul 10)        :c6, 2025-06-23, 2025-07-10
    C-7: Grade Workload (Jul 10-12)             :c7, after k4, 2d
    
    section Buffer
    Final Prep (Jul 15-24)                      :buffer, after k8, 9d
    Assignment Date                              :milestone, assign, 2025-07-24, 0d
```

## Key Dates

| Date | Day | Milestone |
|------|-----|-----------|
| **June 18** | Wed | TODAY - Project starts |
| **June 20** | Fri | SN Student Instance + K WL Config due |
| **June 23** | Mon | C Development starts |
| **June 27** | Fri | K ICE Package due |
| **July 4** | Fri | SN Instance Ready |
| **July 10** | Thu | K Workload execution + C Development complete |
| **July 15** | Tue | **CODON COMPLETE** |
| **July 24** | Thu | **WL1 ASSIGNMENT** |

## Team Legend
- **SN** = ServiceNow
- **K** = Kura  
- **C** = Codon

## Critical Path
1. **SN-1** → **K-2** → **SN-3** → **K-4** → **C-7** → **K-8**
2. **K-5** and **C-6** run in parallel
3. **9-day buffer** for final preparation

---
*Ready to copy into GitHub README.md*
