# Genetic Algorithm for Combinatorial Optimization

This repository contains a Python implementation of a **Genetic Algorithm (GA)** designed to solve the **0/1 Knapsack Problem**. This project serves as an exploration into heuristic optimization and the application of evolutionary strategies to structured, high-dimensional search spaces.

## 📌 Project Motivation
In computational research, we often encounter "NP-hard" problems where an exhaustive search for the optimal solution is mathematically impossible within a reasonable timeframe. The Knapsack Problem is a classic example. This project demonstrates how **stochastic optimization**—inspired by biological evolution—can efficiently converge on near-optimal solutions by navigating complex data manifolds.



## 🧬 Evolutionary Methodology
The solver mimics the principles of natural selection through a cyclical process:

1.  **Population Encoding**: Potential solutions are represented as bit-strings (chromosomes), where each bit corresponds to the inclusion or exclusion of a specific item.
2.  **Fitness Function**: Each candidate is evaluated based on total value. A heavy penalty is applied to "individuals" that violate the weight constraint, effectively removing them from the gene pool.
3.  **Tournament Selection**: A probabilistic approach is used to select the strongest parents for the next generation, maintaining a balance between exploitation (using known good solutions) and exploration (searching new areas).
4.  **Crossover & Mutation**: 
    * **Single-Point Crossover** recombines parental data to produce offspring.
    * **Bit-flip Mutation** introduces random noise, preventing the algorithm from getting stuck in local optima (sub-optimal solutions).



## 🛠️ Technical Stack
* **Language**: Python 3.x
* **Libraries**: 
    * `Pandas`: For structured item management and data handling.
    * `Matplotlib`: For visualizing the convergence of the optimization process.
    * `Random`: For implementing stochastic evolutionary operators.

## 📈 Analysis & Convergence
The algorithm tracks the **Best Fitness** across generations. A typical run demonstrates a sharp logarithmic increase in value before plateauing, signifying that the population has converged toward a global optimum.



## 🚀 How to Use
1. **Clone the repository**:
   ```bash
   git clone [https://github.com/YOUR_USERNAME/Genetic-Algorithm-Knapsack-Solver.git](https://github.com/YOUR_USERNAME/Genetic-Algorithm-Knapsack-Solver.git)
