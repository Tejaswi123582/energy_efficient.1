**Energy-Optimized Task Scheduler (EOTS)**  

**Overview**  
The Energy-Optimized Task Scheduler (EOTS) is a Python-based project that dynamically adjusts CPU frequency levels to optimize energy consumption while ensuring tasks meet their deadlines. The scheduler utilizes various scheduling algorithms to manage task execution efficiently. It features a graphical interface built with Tkinter and provides Gantt chart visualizations using Matplotlib to help users analyze task execution patterns.  

**Key Features**  
**Multiple Scheduling Algorithms:** Implements Priority Scheduling, Earliest Deadline First (EDF), Round Robin, and Hybrid Energy-Aware Priority Scheduling.  
**Dynamic CPU Frequency Adjustment:** The system modifies CPU frequency based on task priority and available slack time to optimize energy efficiency.  
**Multi-Core CPU Simulation:** Distributes tasks across multiple CPU cores to simulate real-world scheduling scenarios.  
**Energy Consumption Tracking:** Monitors and logs the power usage per core to provide insights into energy efficiency.  
**Graphical Interface:** Uses Tkinter to allow users to configure tasks, manage cores, and visualize scheduling behavior.  
**Gantt Chart Visualization:** Displays a graphical representation of task execution over time.  
**Execution Logging:** Captures detailed logs of task execution, including start and end times, core assignments, and energy usage.  

**Dependencies**  
To run the EOTS, ensure you have the following Python libraries installed:  
sh
pip install matplotlib tkinter
  

**Usage**  
Execute the scheduler using:  
```sh
python cpu_scheduling.py
```  

**Interface**  
**Task Configuration:** Allows users to define task priorities, execution times, and deadlines for scheduling.  
**Core Management:** Displays CPU core utilization and associated energy consumption metrics.  
**Gantt Chart:** Provides a visual timeline of task execution across CPU cores.  
**Execution Logs:** Tracks task execution details, including frequency adjustments and energy consumption patterns.  

## **CPU Frequency Levels**  
EOTS dynamically adjusts CPU frequency based on available slack time and task urgency to optimize energy usage:  
**Low (0.8 GHz, power: 0.5 units, green):** Used for tasks with high slack time to conserve energy.  
**Mid (1.2 GHz, power: 1.0 units, yellow):** Balances energy efficiency and performance for moderate slack.  
**High (2.0 GHz, power: 2.0 units, red):** Used for urgent tasks with tight deadlines, prioritizing performance over energy savings.  

## **Scheduling Algorithms**  
**Priority Scheduling:** Tasks with higher priority execute first, ensuring critical tasks are processed promptly.  
**Earliest Deadline First (EDF):** Prioritizes tasks closest to their deadline, preventing deadline misses.  
**Round Robin:** Allocates fixed time slices to tasks in a cyclic order, promoting fairness in task execution.  
**Hybrid Energy-Aware Priority Scheduling:** Dynamically adjusts CPU frequency based on task priority and available slack time, achieving an optimal balance between energy efficiency and performance.  

## **Future Enhancements**  
- Implement machine learning-based scheduling optimizations.  
- Introduce real-time monitoring and predictive analytics.  
- Extend support for heterogeneous multi-core architectures.  
- Improve the graphical interface for enhanced user interaction and real-time updates.  

