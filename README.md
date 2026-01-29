# Smart City Simulation for Emergency Resource Management

A C++ based simulation that optimizes emergency response times in a smart city environment. This project utilizes graph theory and dynamic data structures to manage resources, calculate shortest paths, and handle real-time traffic updates.

![City Graph](docs/logic_diagram.png)

## 🚀 Key Features

* **Optimal Pathfinding:** Uses **Dijkstra’s Algorithm** to calculate the shortest route between critical locations (Hospitals, Fire Stations, Police Stations).
* **Dynamic Task Prioritization:** Implements a **Binary Search Tree (BST)** to queue and process emergency tasks based on urgency and priority.
* **Traffic Simulation:** Features a dynamic weight adjustment system that recalculates travel time based on real-time traffic conditions (Light, Moderate, Extreme).
* **City Graph:** Models the city layout using an **Undirected Graph** with an adjacency list for efficient spatial data management.

## 🛠️ Tech Stack

* **Language:** C++
* **Core Concepts:** Graph Theory, BST, Priority Scheduling, Linked Lists.

## ⚙️ How It Works

The system represents the city as a graph where:
* **Nodes** = Locations (Town Hall, Hospital, etc.)
* **Edges** = Roads with associated weights (Distance/Traffic).

When an emergency occurs, the system:
1.  Inserts the task into a **BST** based on priority (Fire > Robbery > Traffic).
2.  Calculates the shortest path from the nearest responder using **Dijkstra's Algorithm**.
3.  Adjusts for traffic delays if specified by the user.

## 📂 Project Structure

| File | Description |
| :--- | :--- |
| `src/main.cpp` | Core logic for Graph, BST, and Traffic systems. |
| `src/map.txt` | Data file containing city topology (Nodes & Distances). |
| `docs/input_guide.txt` | Guide on how to input location names correctly. |

## 👥 Authors

* **Mian Moiz Ud Din**
* **Tayyab Shajehan**
