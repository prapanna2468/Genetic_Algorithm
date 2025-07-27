#Genetic Algorithm for Smart Grid Energy Optimization
This project implements a Genetic Algorithm (GA) to solve a constrained optimization problem focused on smart grid energy distribution. It demonstrates how heuristic optimization techniques can minimize costs, reduce losses, and fulfill energy demand effectively in a real-world scenario.

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

