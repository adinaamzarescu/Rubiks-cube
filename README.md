#  Rubik's Cube Solver
## Copyright 2024 Adina Amzarescu

## Description

This project investigates and compares different algorithms for solving a 2×2×2 Rubik's Cube, also known as the "Pocket Cube". It includes a detailed study of the A* algorithm, Bidirectional BFS, and Monte Carlo Tree Search (MCTS), offering a rich analysis of their methodologies and efficiencies.

## Installation

To set up the project, install the necessary dependencies:

`
pip install numpy seaborn networkx matplotlib
`

## Usage

Run the `Rubiks_cube.ipynb` notebook to interact with the algorithms. The notebook provides a detailed implementation, comparative analysis, and visualizations of the cube states and algorithm performances.

## Detailed Features

### In-Depth Analysis of Algorithms

#### 1. **A* Algorithm**
- **Overview**: A popular search algorithm used for pathfinding and graph traversal, ideal for solving puzzles like the Rubik's Cube.
- **Implementation**: Utilizes heuristic functions to estimate the 'cost' from the current state of the cube to the solved state.
- **Heuristic Function**: A crucial part of the implementation, enhancing the efficiency of the A* algorithm.
- **Efficiency**: Effective in scenarios where the solution path is not excessively long and the heuristic is well-optimized.

#### 2. **Bidirectional BFS**
- **Overview**: A search strategy that operates from both the initial state and the goal state.
- **Application**: Simultaneously explores moves from the scrambled and solved states.
- **Advantages**: Reduces the time and resources needed to find the solution path.

#### 3. **Monte Carlo Tree Search (MCTS)**
- **Overview**: A heuristic search algorithm known for its effectiveness in large search spaces.
- **Mechanism**: Balances exploring new moves and choosing moves with known high win rates.
- **Rubik's Cube Application**: Useful in complex scenarios with vast search spaces.
- **Performance**: Depends on its ability to balance exploration with exploitation.

### General Features
- **Visualization Tools**: Includes tools to represent the state of the Rubik's Cube and the performance of algorithms.
- **Comparative Analysis**: Measures various metrics to compare the performance of different algorithms.

### Technical Aspects
- **Python Libraries**: Uses libraries like `numpy`, `matplotlib`, `seaborn`, and `networkx`.
- **Code Structure**: Structured into 15 code cells covering various aspects of the project.

## Test Cases and Practical Scenarios

The project includes several test cases to evaluate the performance of the algorithms:
- **Case 1**: "R U' R' F' U"
- **Case 2**: "F' R U R U F' U'"
- **Case 3**: "F U U F' U' R R F' R"
- **Case 4**: "U' R U' F' R F F U' F U U"
- **C Values**: [0.5, 0.1]
- **Budget Values**: [1000, 2000, 5000, 20000]

## License

This project is released under the MIT License. For more details, see the [LICENSE](LICENSE) file.
