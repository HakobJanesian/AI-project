# Nonogram Solver: A Constraint Satisfaction Approach

## Abstract
This project explores the application of various algorithms to solve Nonograms, popular Japanese logic puzzles also known as Hanjie, Paint by Numbers, or Griddlers. We approach Nonograms as a Constraint Satisfaction Problem (CSP) and investigate different methodologies including Integer Linear Programming, Genetic Algorithms, and Depth First Search. The primary goal is to fill a grid based on constraints that determine the placement of contiguous blocks, revealing a hidden image upon completion.

## Introduction
Nonograms pose a significant challenge in computational logic, classified as an NP-complete problem. The objective is to color cells in a matrix based on provided row and column descriptions, maintaining a constraint of at least one white cell between consecutive black segments. Our project aims to solve these puzzles efficiently, considering various algorithmic approaches.

## Structure
1. **Literature Review**: Analysis of existing solutions such as iterative search, ILP, GA, and depth-first search.
2. **Algorithm Description**: Explanation of our main algorithm for solving the puzzles.
3. **Results Overview**: Presentation of the solved puzzles and corresponding runtimes.

## Literature Review
We delve into three prominent approaches:
1. **Depth First Search**: Exploring all feasible block arrangements in each line.
2. **Integer Linear Programming and Iterative Search**: A hybrid model combining iterative methods with ILP for enhanced performance.
3. **Genetic Algorithm**: Developed by Professor Wouter Wiggers, focusing on mutation, selection, and crossover operations.

## Numerics and Solution
Our solution, coded in Python using libraries like Pandas, Numpy, and Matplotlib, treats nonograms as CSPs. The algorithm enforces row constraints, eliminates domain values that violate constraints, and applies backtracking with forward checking for efficient search.

## Algorithm
The core algorithm involves:
1. Enforcement of row constraints.
2. Traversal and elimination of invalid domain values.
3. Recursive backtracking with consistency checks and forward checking.

## Results
The algorithm's efficacy is demonstrated across puzzles of varying sizes. Execution times ranged from 0.1 seconds for smaller puzzles to 1.2 minutes for larger, more complex ones.

## Conclusion
While small nonograms are solved rapidly, larger puzzles require more time, highlighting the need for further optimization in inference and search processes. The current goal is to enhance the algorithm's time efficiency.

## Further Work
Future improvements may include heuristic modifications to the backtracking algorithm, like backjumping, to avoid rediscovering dead ends, thereby solving nonograms more efficiently.

## Bibliography
The bibliography section includes references to all the literature and studies reviewed and utilized in this project.
