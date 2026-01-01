# Smart Resource Allocation & Scheduling System

**Tools Used:** Python, Jupyter Notebook, Pandas, Matplotlib  

---

## Project Overview

This project implements a **logic-driven scheduling engine** designed to efficiently allocate multiple tasks across limited resources.  
The main goal is to **minimize idle time** and **maximize resource utilization** by allowing resources to handle **non-overlapping tasks** based on skill, availability, and priority.  

The system simulates **48 resources** with different skills and working hours, and **300+ tasks** with varying priorities, durations, and skill requirements. Edge cases are included to validate reliability and robustness.

---

## Objectives

- Develop a **baseline scheduling algorithm** representing a legacy allocation system.  
- Implement an **optimized scheduler** that allows **non-overlapping task reuse** per resource.  
- Measure and reduce **idle time** for resources.  
- Validate the system with edge cases and large-scale simulated data.  
- Visualize improvements in resource utilization.

---

## Methodology

1. **Data Generation**  
   - Resources and tasks are generated with attributes like skills, time windows, and priorities.  
   - Edge cases include invalid time windows and unavailable skills to test robustness.  

2. **Baseline Scheduler**  
   - Each resource is assigned at most one task.  
   - Assignments based on skill match and priority.  
   - Calculates total idle hours for all resources.  

3. **Optimized Scheduler**  
   - Allows multiple tasks per resource if time windows do not overlap.  
   - Assignments consider skill match, availability, and task priority.  
   - Calculates total idle hours after optimized scheduling.  

4. **Metrics**  
   - **Baseline Idle Hours:** Total idle time for resources in the baseline allocation.  
   - **Optimized Idle Hours:** Total idle time for resources in the optimized allocation.  
   - **Idle Time Reduction (%)** = `(Baseline Idle - Optimized Idle) / Baseline Idle * 100`  

5. **Visualization**  
   - Bar charts compare **baseline vs optimized idle hours** for clarity.

---

## Key Results

- Baseline idle hours: Example ~214  
- Optimized idle hours: Example ~55  
- **Idle Time Reduction:** ~74%  

The optimized scheduler significantly reduces idle time, improving overall resource utilization.  

---

## Conclusion

The Smart Resource Allocation & Scheduling System demonstrates a **scalable and robust scheduling solution**:

- Non-overlapping allocation maximizes efficiency.  
- Edge-case validation ensures reliability.  
- Idle time and resource utilization metrics provide clear evidence of improvement.  

This system can be further extended to include **predictive scheduling, dynamic resource addition, or task dependencies**, making it suitable for real-world operations in IT, manufacturing, or service management.  

---

## How to Use

1. Open the `Resource_Scheduler.ipynb` notebook in **Jupyter Notebook**.  
2. Run all cells sequentially to simulate resource allocation and observe **idle time reduction**.  
3. Visualizations will be generated automatically.  

---

## Author

**Shouray Soni** – B.Tech CSE / ECE Student  
GitHub: https://github.com/Shouray1104
