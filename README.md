Genetic Algorithm for Smart Grid Energy Distribution
This project demonstrates the application of a Genetic Algorithm (GA) to optimize the distribution of power among four generators in a smart grid system. The aim is to satisfy a specific power demand while minimizing the total cost of generation and ensuring that each generator operates within its allowable output limits. The approach used in this assignment involves representing potential solutions as chromosomes, applying genetic operations to evolve these solutions over generations, and evaluating their performance using a custom fitness function with penalties for constraint violations.

In this problem, each chromosome consists of four genes, each representing the power output of a generator. These outputs must lie within predefined minimum and maximum bounds. Additionally, the total output from all generators must meet or exceed a required demand. The GA operates by first initializing a population of such chromosomes with random values within valid ranges. It then evaluates each chromosome based on a cost function that models the real-world cost associated with power generation at each generator. If a chromosome fails to meet the demand or violates generator constraints, it is heavily penalized in the fitness evaluation.

The genetic algorithm proceeds by selecting parent chromosomes using a roulette wheel selection strategy, which biases the selection towards chromosomes with better fitness (i.e., lower cost). A single-point crossover technique is used to recombine genes from two parents and produce new offspring. Mutation is applied with a certain probability to randomly alter the power output of a gene within valid bounds, encouraging diversity in the population and helping to explore the solution space. An elitism strategy is also adopted to preserve the best solution from each generation, ensuring that the global best solution is not lost during the evolutionary process.

Over a defined number of generations, the GA iteratively improves the population by generating new candidate solutions and selecting the most promising ones. At the end of the process, the best chromosome represents the optimal or near-optimal configuration of generator outputs that minimize the total cost while satisfying the demand and adhering to all constraints. A convergence plot is also generated to visualize how the cost improves over generations.

This assignment helped solidify theoretical understanding of evolutionary algorithms and how they can be applied to solve real-world constrained optimization problems. It covered key GA components such as chromosome encoding, selection pressure, fitness evaluation, crossover and mutation, and the use of penalties to handle constraint violations. The project demonstrates how biologically inspired algorithms can be effectively used to optimize complex systems in the field of energy management.
Overview
This notebook simulates how a Genetic Algorithm can optimize energy distribution by:

Defining a chromosome structure that encodes generator power outputs.

Creating a fitness function to evaluate cost efficiency, power losses, and unmet demand.

Incorporating GA operations: selection, crossover, mutation, and elitism.

Enforcing constraints such as power limits and demand satisfaction using penalty functions.

The approach balances exploration and exploitation to achieve an optimal or near-optimal solution within acceptable computational limits.

Features
Customizable GA parameters (population size, generations, mutation rate)

Constrained optimization using penalty functions

Visualization of convergence (fitness over generations)

Student-friendly code with stepwise logic and inline explanations

File Structure
bash
Copy
Edit
Genetic_Algorithm.ipynb  # Main Jupyter Notebook with implementation
README.md                # Project overview and instructions (you are reading this)
How to Run
Clone the repository or upload to Google Colab:

bash
Copy
Edit
git clone https://github.com/<your-username>/genetic-algorithm-energy-optimization.git
Open the notebook Genetic_Algorithm.ipynb in Jupyter Notebook or Google Colab.

Run all cells sequentially to simulate the optimization process.

Dependencies
Python 3.x

NumPy

Matplotlib

(Optional) Jupyter Notebook or Google Colab

Note: Please make sure to update file paths if any input/output files are used, as hardcoded paths might not work on all systems.

Output
Final optimized generator power distribution

Minimum cost considering losses and constraints

Convergence graph showing fitness value over generations

Learning Outcomes
Through this project, I learned:

How to formulate a real-world optimization problem for a GA.

The importance of fitness functions and penalty-based constraints.

Tuning GA parameters for better convergence.

Author
Prapanna Upadhyay
Student ID: 0371357
BCS Program

License
This project is intended for academic purposes only. Do not use it commercially without permission.

