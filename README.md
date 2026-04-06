# mapreduce-graph-algorithms
This repository contains implementations of large-scale graph algorithms using the MapReduce framework. The project specifically focuses on applying the strategies outlined in the research paper: **"Design Patterns for Efficient Graph Algorithms in MapReduce."**

## Overview
Processing massive graphs (like social networks or web crawls) requires efficient distributed computing. This project explores how to structure graph data and MapReduce jobs to minimize overhead and maximize parallel performance.

## Algorithms Implemented
**Breadth-First Search (BFS):** Used for finding shortest paths in unweighted graphs.
**PageRank:** An iterative algorithm used to rank the importance of nodes based on the link structure.
**Graph Representations:** Implementation of adjacency lists and node state tracking within MapReduce tuples.

## Design Patterns Used
To optimize these algorithms, we implemented the following patterns:
**In-Mapper Combining:** Reducing the number of intermediate key-value pairs to save network bandwidth.
**Schimmy Design Pattern:** Efficiently joining graph structure with ranking data to avoid shuffling the entire graph in every iteration.

## Repository Structure
`PageRankBFS_updated.ipynb`: Main Jupyter Notebook containing the Python/PySpark implementation and analysis.

## How to Run ?
1. Clone the repository:
   ```bash
   git clone [https://github.com/yourisev/mapreduce-graph-algorithms.git](https://github.com/yourisev/mapreduce-graph-algorithms.git)
   ```
2. Open `PageRankBFS_updated.ipynb` in a Jupyter environment (or Google Colab).

3. Ensure you have the required dependencies (Spark/PySpark) installed to execute the MapReduce simulations.
