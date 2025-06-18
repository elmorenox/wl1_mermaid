# WL1 Project Schedule - Codon Complete by July 15th

## Project Timeline

```mermaid
%%{init: {'theme':'base', 'themeVariables': {'primaryColor': '#8fbc8f', 'primaryTextColor': '#000', 'doneTaskBkgColor': '#cd853f', 'doneTaskTextColor': '#000', 'activeTaskBkgColor': '#808080', 'activeTaskTextColor': '#fff', 'taskBkgColor': '#8fbc8f', 'taskTextColor': '#000'}}}%%
gantt
    title WL1 Project Timeline
    dateFormat YYYY-MM-DD
    axisFormat %m/%d
    
    section All Tasks
    SN Delivers Student Instance          :sn, sn1, 2025-06-18, 2025-06-20
    Kura Defines WL Config                :done, k5, 2025-06-18, 2025-06-20
    Kura Delivers ICE Package             :done, k2, after sn1, 7d
    SN Delivers Instance Ready            :sn, sn3, after k2, 7d
    Codon Develops Grading                :active, c6, 2025-06-23, 2025-07-10
    Kura Executes Workload                :done, k4, after sn3, 6d
    Codon Grades Workload                 :active, c7, after k4, 2d
    Grading Approved by Kura              :done, k8, after c7, 3d
    WL1 Assignment                        :milestone, assign, 2025-07-24, 0d
```
