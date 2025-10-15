#  OS Lab Simulator (Operating System Visualizer)

###  Course: TCS-502 — Operating System  
###  Team OS-V T262 — *"Challengers"*

> A web-based simulator designed to **visualize core Operating System concepts** like CPU Scheduling, Memory Management, Deadlock Handling, and File System operations.  
> Built using **HTML, CSS, JavaScript**, and **Python (Flask)** for algorithm computation and backend API integration.

---

##  Project Overview

The **OS Visualizer** provides an **interactive learning experience** for students to understand how OS algorithms work internally — through **real-time simulations and visual outputs**.

Instead of reading static diagrams, users can **add processes, allocate memory, run algorithms**, and see dynamic charts and Gantt timelines appear instantly.

---

##  Features

| Module | Description | Status |
|---------|--------------|--------|
| **CPU Scheduling** | Visualizes FCFS, SJF, and Round Robin algorithms with Gantt charts and metrics. | ✅ Completed |
| **Memory Management** | Simulates First Fit, Best Fit, and Worst Fit allocation methods. | ✅ Completed |
| **Deadlock Detection & Avoidance** | Implements Resource Allocation Graph and Banker’s Algorithm visualization. | 🚧 In Progress |
| **File System Visualization** | Interactive file hierarchy simulator for create/delete/search operations. | ⏳ Pending |
| **UI Design & Integration** | Unified dark-themed, responsive UI with interactive controls. | 🚧 In Progress |

---

##  Project Architecture

### **Client-Server Model**

- **Frontend (Client)**:  
  Built using HTML, CSS, and JavaScript.  
  - Displays simulation UI (tables, forms, Gantt charts).
  - Uses asynchronous API calls (`fetch`) to communicate with Flask backend.
  - Visualized through dynamic DOM manipulation.

- **Backend (Server)**:  
  Implemented in **Python Flask**.  
  - Handles algorithm logic for CPU scheduling, memory allocation, and deadlock avoidance.  
  - Returns computed data (Gantt chart positions, metrics, safety sequences) in JSON format.

### **Data Flow**
```text
User Input → Frontend (JS) → Flask API (Python) → JSON Response → Visualization (DOM)
