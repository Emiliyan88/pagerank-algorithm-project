# PageRank Algorithm Project

This project explores the mathematical foundations and Python implementation of the PageRank algorithm.
The goal of the project is to understand how mathematics, graph theory and probability can be used to rank nodes in a network.
The project includes a step-by-step implementation of the algorithm and several experiments demonstrating how PageRank behaves on different graph structures.

## Project goals

- Understand the mathematics behind PageRank
- Implement the algorithm in Python
- Analyze its behavior on different network structures
- Visualize ranking results

## How the PageRank algorithm works

PageRank models the web as a directed graph:

- nodes represent web pages
- edges represent hyperlinks between pages

The importance of a page depends on the importance of the pages linking to it.

The PageRank formula is:

PR(i) = (1 − d)/N + d Σ(PR(j)/L(j))

Where:

- PR(i) – PageRank of page i
- d – damping factor (usually 0.85)
- N – total number of pages
- PR(j) – PageRank of page j linking to page i
- L(j) – number of outgoing links from page j

The algorithm repeatedly updates the PageRank values until they converge.

## Technologies

- Python
- NumPy
- NetworkX
- Matplotlib

## Project Structure

pagerank-algorithm-project
│
├── page_rank_algorithm.ipynb
└── README.md

## Experiments

The project includes several experiments:

- PageRank computation on small graphs
- Comparison with NetworkX implementation
- Convergence analysis
- Experiments with different network structures

## Results

The PageRank algorithm successfully ranks nodes based on their structural importance in the network.
The results from our custom implementation closely match the values produced by the NetworkX implementation, confirming the correctness of the algorithm.

## Author

Emiliyan

## Sources
1. Page, L., Brin, S. (1998). The PageRank Citation Ranking: Bringing Order to the Web.
2. NetworkX Documentation – PageRank Algorithm.
3. Introduction to Algorithms – Cormen, Leiserson, Rivest, Stein.
4. Wikipedia – PageRank Algorithm.
5. Chat GPT