# TSP-
Travelling salesman problem using MIP
Traveling Salesman Problem (TSP) - MIP Solution

Overview

This repository contains an implementation of the Traveling Salesman Problem (TSP) using Mixed-Integer Programming (MIP). The solution is formulated as an optimization problem and solved using a mathematical programming solver.

Problem Statement

The Traveling Salesman Problem (TSP) is a classic combinatorial optimization problem where a salesman must visit a set of cities exactly once and return to the starting city while minimizing the total travel cost (e.g., distance or time).

Approach

This implementation models the TSP as a Mixed-Integer Linear Program (MILP):

Decision Variables: Binary variables indicating whether an edge is included in the tour.

Objective Function: Minimize the total travel cost.

Constraints:

Each city must be visited exactly once.

Subtour elimination constraints to ensure a single tour.

Requirements

To run the implementation, you need the following dependencies:

Python 3.x

pulp (Python library for linear programming)

A solver such as Gurobi, CBC, or CPLEX

Install dependencies using:

pip install pulp

Usage

Run the script with:

python tsp_mip.py

You can modify the distance matrix in the script to test different datasets.

Example Output

Optimal Tour: [0, 2, 1, 3, 0]
Total Cost: 150

Notes

The implementation ensures subtour elimination using the MTZ (Miller-Tucker-Zemlin) formulation.

The solver used can be changed based on availability and performance needs.

License

This project is licensed under the MIT License. Feel free to modify and use it!

Author

Ladan Farbiz
