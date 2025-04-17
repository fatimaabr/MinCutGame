# 🧩 Minimum Cut Game (MCG) – Optimization Project

Author: Fatima Aboura
Tool: IBM CPLEX Solver
Format: Jupyter Notebook (MCG.ipynb)

# 📌 Problem Statement
The Minimum Cut Problem (MCP) is a classical graph theory problem that involves partitioning a graph's nodes into two disjoint sets such that the sum of the capacities of the edges crossing the partition (the cut) is minimized.

In this project, we study a more advanced variant called the Min Cut Game (MCG). This model introduces agents—a specific subset of nodes—and incorporates a stability condition to the classic problem. The goal is to find a minimum capacity cut that also satisfies agent-related constraints, ensuring fair and stable allocation of edge flows.

# 🎯 Objectives
Minimize the capacity of a cut in a given graph.

Ensure that the stability condition for agents is respected:

Agents must receive a fair and balanced distribution of edges after the cut.

The structure remains stable and efficient for flow distribution or network operations.

Model and solve this constrained version of the Min Cut Problem using Integer Programming.

# 🧠 Key Concepts
Graph Cut: Partition of graph nodes into two sets where the cut-set consists of edges crossing between the sets.

Capacity: Each edge has a weight (capacity), and the goal is to minimize the sum of cut-edge capacities.

Agents: Specific nodes with additional fairness/stability constraints.

Stability Condition: Ensures that no agent would benefit by unilaterally changing their side of the cut (i.e., Nash-like stability).

NP-hardness: The MCG problem is computationally hard and cannot be solved in polynomial time for all cases.

# 🛠️ Methodology
1. Mathematical Modeling
Decision variables represent the assignment of nodes to partitions.

Binary variables capture edge crossing status.

Stability constraints ensure agent fairness.

Objective function: Minimize the total capacity of edges in the cut.

2. Implementation with CPLEX
The model is implemented using IBM's CPLEX Optimization Studio.

Steps include:

Defining decision variables.

Coding objective functions.

Incorporating stability constraints.

Solving and analyzing the results.

# 📊 Applications
The Min Cut Game framework can be applied in:

Network Design & Load Balancing

Social Network Analysis

Fair Resource Allocation

Image Segmentation

Clustering and Partitioning Problems

# 📈 Results & Analysis
The solution provides:

The structure of the optimal cut.

The distribution of agents across partitions.

Verification of stability conditions.

Insights into the computational complexity and solution time.

# 🔮 Future Directions
Explore heuristic or metaheuristic approaches for large-scale instances.

Consider dynamic or time-varying graphs.

Extend to multi-agent or multi-level fairness constraints.

Integrate visualization tools for better interpretation.
