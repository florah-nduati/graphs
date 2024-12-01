# Graph Theory and Dynamic Programming: Detailed Notes

## Table of Contents
1. [Introduction](#introduction)
    - Purpose
    - Scope
    - Prerequisites
2. [Graphs Overview](#graphs-overview)
    - What is a Graph?
    - Types of Graphs
3. [Directed vs. Undirected Graphs](#directed-vs-undirected-graphs)
    - Directed Graphs (Digraphs)
    - Undirected Graphs
4. [Weighted vs. Unweighted Graphs](#weighted-vs-unweighted-graphs)
    - What is a Weighted Graph?
    - What is an Unweighted Graph?
5. [Dynamic Programming](#dynamic-programming)
    - What is Dynamic Programming?
    - Key Concepts of Dynamic Programming
    - Applications of Dynamic Programming
6. [Conclusion](#conclusion)

---

## 1. Introduction

### Purpose
This document serves as a detailed guide to understanding the concepts of directed vs. undirected graphs, weighted vs. unweighted graphs, and dynamic programming. It provides an in-depth explanation of these fundamental concepts along with examples and their practical applications.

### Scope
The document covers:
- **Directed vs. Undirected Graphs**: Definitions, properties, and use cases.
- **Weighted vs. Unweighted Graphs**: Definitions, how to represent them, and their applications.
- **Dynamic Programming**: Explanation, key principles, and practical applications in graph algorithms and optimization problems.

### Prerequisites
Familiarity with basic programming concepts and graph theory will be beneficial for understanding the content. Knowledge of algorithms and data structures (especially in Python or similar languages) is recommended.

---

## 2. Graphs Overview

### What is a Graph?

A **graph** is a collection of nodes (vertices) and edges (connections between pairs of nodes). Graphs are a fundamental data structure used to represent networks, relationships, and structures in various domains like social networks, computer networks, transportation systems, and more.

### Types of Graphs

Graphs can be classified based on various properties:
1. **Directed vs. Undirected**: Refers to whether edges have direction.
2. **Weighted vs. Unweighted**: Refers to whether edges have weights (costs or distances).
3. **Cyclic vs. Acyclic**: Whether the graph contains cycles (closed paths).
4. **Connected vs. Disconnected**: Whether all nodes are reachable from each other.

---

## 3. Directed vs. Undirected Graphs

### Directed Graphs (Digraphs)

A **directed graph** (digraph) consists of edges that have direction. Each edge is an ordered pair of nodes, indicating a one-way relationship.

- **Notation**: An edge from node A to node B is represented as `(A, B)`.

#### Properties:
- **Edge Direction**: The edges are directed from one node to another.
- **Outdegree**: The number of outgoing edges from a node.
- **Indegree**: The number of incoming edges to a node.

#### Use Cases:
- Modeling one-way streets or traffic routes.
- Representing follower-following relationships in social media.
- Network routing algorithms.

### Undirected Graphs

An **undirected graph** has edges with no direction. The relationship between two nodes is mutual and bidirectional.

- **Notation**: An edge between nodes A and B is represented as `{A, B}`.

#### Properties:
- **No Edge Direction**: The relationship is symmetric between nodes.
- **Degree**: The number of edges incident to a node.

#### Use Cases:
- Representing bidirectional roads in a city.
- Friendship relationships in social networks (e.g., Facebook).
- Checking graph connectivity.

---

## 4. Weighted vs. Unweighted Graphs

### What is a Weighted Graph?

A **weighted graph** assigns a numerical value (weight) to each edge, often representing cost, distance, or capacity. 

- **Notation**: An edge between nodes A and B with weight `w` is represented as `(A, B, w)`.

#### Properties:
- **Weight**: Each edge has a numerical cost or value.
- **Use Cases**: Used in problems requiring optimization (shortest paths, minimum spanning trees, etc.).

#### Use Cases:
- Shortest path algorithms (e.g., Dijkstra’s, Bellman-Ford).
- Network flow problems.
- Resource optimization (e.g., minimum spanning tree).

### What is an Unweighted Graph?

An **unweighted graph** does not assign any weights to its edges. All edges are treated equally, often representing a simple relationship or connection.

- **Notation**: An edge between two nodes is simply `{A, B}`.

#### Properties:
- **No Weight**: Every edge is treated equally.
- **Use Cases**: Simplified graph problems where edge weights are not considered.

#### Use Cases:
- Graph traversal algorithms (e.g., BFS, DFS).
- Connectivity checks in a network.
- Social network analysis (e.g., degree of separation).

---

## 5. Dynamic Programming

### What is Dynamic Programming?

**Dynamic Programming (DP)** is a method of solving complex problems by breaking them down into simpler overlapping subproblems. It optimizes by storing the results of subproblems (memoization) to avoid redundant calculations.

#### Key Concepts of Dynamic Programming:
1. **Overlapping Subproblems**: The problem can be divided into smaller subproblems that are solved multiple times.
2. **Optimal Substructure**: The solution to the overall problem can be constructed from the solutions to its subproblems.

#### Techniques:
1. **Memoization**: Storing results of subproblems for reuse.
2. **Tabulation**: Building solutions iteratively and filling a table (usually an array or matrix) to avoid recomputation.

### Applications of Dynamic Programming

DP is applied in optimization problems that can be decomposed into smaller subproblems. Examples include:

1. **Shortest Path Problems**:
   - **Floyd-Warshall Algorithm**: Computes the shortest paths between all pairs of nodes in a weighted graph.
   - **Bellman-Ford Algorithm**: Solves the single-source shortest path problem, even with negative weights.
   
2. **Longest Path Problems**:
   - Problems like longest increasing subsequence (LIS), longest common subsequence (LCS).

3. **Knapsack Problems**:
   - Optimal resource allocation problems, such as the 0/1 knapsack problem.

4. **Matrix Chain Multiplication**:
   - Finding the most efficient way to multiply matrices in sequence.

5. **Graph Problems**:
   - **Shortest Path in Graphs**: DP can be applied in finding the shortest path in weighted graphs (using algorithms like Dijkstra).
   - **Longest Path in Directed Acyclic Graphs (DAGs)**: DP can be used to compute the longest path in a DAG.

---

## 6. Conclusion

This document has provided an in-depth look at fundamental graph theory concepts such as **directed vs. undirected graphs**, **weighted vs. unweighted graphs**, and **dynamic programming**. These concepts form the backbone of many algorithms and optimization problems, making them essential to understand when working with graphs and solving complex problems in areas like network analysis, social media, and pathfinding algorithms.

---

## References

- [Introduction to Graph Theory](https://en.wikipedia.org/wiki/Graph_theory)
- [Dynamic Programming](https://en.wikipedia.org/wiki/Dynamic_programming)
- [Dijkstra's Algorithm](https://en.wikipedia.org/wiki/Dijkstra%27s_algorithm)
- [Bellman-Ford Algorithm](https://en.wikipedia.org/wiki/Bellman%E2%80%93Ford_algorithm)
