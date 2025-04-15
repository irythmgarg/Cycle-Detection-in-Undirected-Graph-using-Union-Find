# Cycle-Detection-in-Undirected-Graph-using-Union-Find

# 🔁 Cycle Detection in an Undirected Graph

## 🧩 Problem Statement

Given an **undirected graph** with `V` vertices, your task is to **detect if a cycle exists** in the graph.

---

## 🛠️ Approach

We solve this using the powerful **Disjoint Set Union (DSU)** aka **Union-Find** data structure.

### 🔍 Key Concepts:

- Each node belongs to a "set".
- When we connect two nodes:
  - If they are already in the **same set**, a **cycle** exists.
  - Otherwise, we **union** the two sets.
- Use:
  - **Path Compression** for efficient `find`
  - **Union by Rank** to maintain optimal structure

---

## 🧠 Example

### Input: V = 4
adj = [[1, 2], [0, 2], [0, 1, 3], [2]]
output - true

⚙️ Time Complexity:
O(E * α(N)), where α is the inverse Ackermann function

Nearly linear time due to optimizations

🔎 Notes
Only check each edge once using the if (i >= a) trick

Union-Find is extremely effective for cycle detection in undirected graphs

📌 Tags
Graph • Union-Find • Disjoint Set • Cycle Detection • DSU
