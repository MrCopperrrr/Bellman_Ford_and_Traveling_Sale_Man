# Bellman_Ford_and_Traveling_Sale_Man
Discrete_Structures_for_Computing_Assignment

## Traveling Salesman Problem (TSP) Solver using Dynamic Programming with Bitmasking

This repository contains a C++ implementation of a Traveling Salesman Problem (TSP) solver using dynamic programming with bitmasking. This approach provides an efficient way to find the optimal solution for relatively small instances of the TSP.

## Description

The Traveling Salesman Problem (TSP) is a classic NP-hard problem where the goal is to find the shortest possible route that visits each city exactly once and returns to the origin city.

This implementation utilizes dynamic programming with bitmasking to solve the TSP.  Here's a brief overview of the approach:

*   **Dynamic Programming:** The algorithm computes the shortest path from the starting city to every other city, visiting all cities exactly once. It stores and reuses intermediate results to avoid redundant calculations.
*   **Bitmasking:** Bitmasking is used to efficiently represent the set of visited cities. Each bit in the mask corresponds to a city, and the bit is set to 1 if the city has been visited.

## Features

*   C++ Implementation of TSP solver
*   Dynamic Programming with Bitmasking optimization
*   Clear and concise code with comments
*   Example test cases included

## Code Structure

*   `tsp.cpp`: Contains the core TSP solver functions.
    *   `tsp(graph, pos, visited, dp, parent, numVertices)`: The recursive function that calculates the minimum cost path using dynamic programming and bitmasking.
    *   `Traveling(graph, numVertices, startVertex)`:  The main function that initializes the DP table, calls the `tsp` function, and reconstructs the optimal path.
*   `inMat1.txt`: Contains the adjacency matrix representing the distances between cities.

## Input Format

The input is read from the `inMat1.txt` file. The file should contain an adjacency matrix representing the distances between cities. The matrix should be a square matrix with `n` rows and `n` columns, where `n` is the number of cities. Each element `graph[i][j]` represents the distance between city `i` and city `j`.

## Test Cases

The repository includes four test cases. The number of vertices (cities) is set to 12, and the starting vertex is 'A'.


