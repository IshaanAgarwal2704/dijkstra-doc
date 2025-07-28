Overview
This project implements Dijkstra's algorithm, a popular graph algorithm for finding the shortest paths from a source node to all other nodes in a weighted graph.

Code Structure
dijkstra.c	Core implementation of Dijkstra's algorithm.
dijkstra.h	Header file containing function declarations and macros.
main.c	Entry point for running the algorithm with a sample graph.

Key Functions & Their Roles
int minDistance(int dist[], bool sptSet[], int V)
Purpose: Finds the vertex with the minimum distance value from the set of vertices not yet processed.

How it works: Iterates through all vertices and picks the one with the smallest distance.

void dijkstra(int graph[V][V], int src)
Purpose: Implements Dijkstra's algorithm using an adjacency matrix.

How it works:
Initializes distance array.
Calls minDistance repeatedly to find the closest unvisited node.
Updates distances of neighboring vertices.

void printSolution(int dist[], int V)
Purpose: Prints the computed shortest distances from the source to each vertex.

main() in main.c
Purpose: Demonstrates usage of the Dijkstra algorithm with a sample graph.

Understanding the Flow:
User defines a graph using an adjacency matrix.
Calls dijkstra() with the source vertex.
Internally, the algorithm finds shortest paths and prints them.

Summary of Learnings
The project uses static arrays and adjacency matrix representation, suitable for small graphs.
The algorithm follows a greedy approach, choosing the nearest unvisited vertex at each step.
The code is modular, with clear separation between core logic (dijkstra.c) and driver code (main.c)
