# 🚀 CPU Scheduling Visualizer  

## 📌 Overview  
**CPU Scheduling Visualizer** is a **web-based simulator** that allows users to input processes and visualize the execution of various **CPU scheduling algorithms**. It provides a **dynamic and interactive Gantt Chart**, along with **performance metrics** like waiting time and turnaround time. This tool is useful for students and professionals to understand how different scheduling techniques manage process execution.  

---

## 🎯 Features & Functionalities  

### 🔹 1. Process Management  
- Users can **add multiple processes** by specifying:  
  - **Process ID:** Unique identifier for the process (e.g., P1, P2, P3).  
  - **Arrival Time:** The time when the process enters the system queue.  
  - **Burst Time:** The amount of CPU time required for execution.  
  - **Priority:** (Only applicable for **Priority Scheduling**).  
- The following buttons help manage processes:  
  - **Add Process** – Adds a new process to the queue.  
  - **Clear All Processes** – Removes all processes from the table.  

---

### 🔹 2. CPU Scheduling Algorithms Supported  
The tool supports **five different scheduling techniques**:  

#### ✅ **First-Come, First-Served (FCFS)**
- The **earliest arriving process** is executed first.  
- Simple and easy to implement.  
- **Non-preemptive** (once a process starts execution, it runs until completion).  

#### ✅ **Shortest Job First (SJF) (Non-Preemptive)**
- The process with the **shortest burst time** is executed first.  
- Efficient but may cause **starvation** for longer processes.  

#### ✅ **Shortest Job First (SJF) (Preemptive)**
- **Dynamically selects** the process with the shortest remaining burst time.  
- If a **new process** with a **shorter burst time** arrives, the running process is **preempted**.  
- Ensures faster completion for shorter tasks but may **increase overhead**.  

#### ✅ **Priority Scheduling (Non-Preemptive)**
- Each process is assigned a **priority number** (lower number = higher priority).  
- The process with the highest priority executes first.  
- **Starvation** can occur for lower-priority processes.  

#### ✅ **Round Robin (RR)**
- **Time-sharing algorithm** where each process gets a **fixed time quantum** (default: **2 units**).  
- If a process doesn’t finish in its allocated time, it moves to the end of the queue.  
- Prevents **starvation** and ensures **fair CPU allocation**.  

---

### 🔹 3. Gantt Chart Visualization  
- **Graphical representation** of process execution order.  
- Displays the **start time and end time** of each process.  
- **Smooth animations** make it easy to track CPU allocation.  

---

### 🔹 4. Performance Metrics Calculation  
The tool **automatically calculates** the following metrics after scheduling execution:  

#### 📌 **Average Waiting Time (AWT)**  
\[
\text{Waiting Time} = \text{Turnaround Time} - \text{Burst Time}
\]  
- Lower waiting time indicates **better scheduling efficiency**.  

#### 📌 **Average Turnaround Time (TAT)**  
\[
\text{Turnaround Time} = \text{Completion Time} - \text{Arrival Time}
\]  
- Helps measure how **quickly processes complete execution**.  

Both AWT and TAT are displayed in real-time.  

---

### 🔹 5. Session Management (Save & Load)  
- **Save Session** – Stores the current process list and selected scheduling algorithm in **local storage**.  
- **Load Session** – Restores the saved session.  
- Ensures **continuity**, even if the page is refreshed.  

---

## 🛠️ Technologies Used  
- **HTML, CSS, JavaScript** – Frontend development and interactivity.  
- **DOM Manipulation & Event Handling** – Handling user input dynamically.  
- **LocalStorage API** – Saving and loading session data.  

---

## 🏗️ Installation & Setup  
1. **Clone this repository**:  
   ```bash
   git clone https://github.com/your-username/cpu-scheduler-visualizer.git
   cd cpu-scheduler-visualizer
   ```  
2. **Open `index.html` in a web browser**.  

---

## 🔥 Usage Instructions  
1. **Enter process details** (Process ID, Arrival Time, Burst Time, and Priority if required).  
2. **Select a CPU Scheduling Algorithm** from the dropdown.  
3. Click **"Run Scheduler"** to execute the chosen algorithm.  
4. **Observe the Gantt Chart** for execution order.  
5. View **Average Waiting Time** and **Turnaround Time** in real-time.  
6. **Use "Save Session" and "Load Session"** for persistent data.  

---

## 📸 Screenshots  
(Add screenshots of the interface and Gantt chart here.)  

---

## 🤝 Contributing  
Contributions are welcome! Feel free to fork this repository and submit a pull request.  

---

## 📜 License  
This project is licensed under the **MIT License**.  
