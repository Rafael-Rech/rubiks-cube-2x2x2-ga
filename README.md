# 2x2x2 Rubik's Cube Solver Using a Genetic Algorithm

This project implements a **genetic algorithm-based solver for the 2x2x2 Rubik's Cube**, developed as part of a **Natural Computing** subject at university.
The goal is to explore biologically inspired optimization techniques and evaluate their effectiveness in solving combinatorial problems.

---

## Overview

A 2x2x2 Rubik's Cube has **3,674,160 possible states**, making it significantly simpler than a 3x3x3 cube but still complex enough to serve as an interesting benchmark for evolutionary algorithms.

This solver uses a **genetic algorithm (GA)** to evolve candidate move sequences toward a fully solved cube state.
Individuals represent possible solution sequences, and the GA improves them across generations using selection, crossover, and mutation.

---

## Genetic Algorithm Approach

### **Representation**

* Each individual is a sequence of cube moves (e.g., `R`, `R'`, `U`, `U'`, `F`, `F'`, etc.).

### **Fitness Function**

The fitness score is based on the number of correctly placed cubies.

Lower fitness means a better solution.

### **Genetic Operators**

* **Selection:** Random parents are selected.
* **Crossover:** A developed operator that separates the chromosome based on the last point within the movement sequence that improves the fitness. 
* **Mutation:** Exchange mutation, where two positions in the chromosome are swapped.
* **Elitism:** Best individuals carried over to next generation.

---

## Features

* Complete implementation of cube state representation
* Move operations following standard cube notation
* Configurable GA parameters:

  * Maximum generations
  * Population size
  * Chromosome size
  * Number of crossovers per generation
  * Mutation rate
  * Elitism rate
  * Maximum accepted similarity rate
---

## Technologies Used

* **Jupyter Notebook using Python**
---

## How to Run

1. Clone the repository:

   ```
   git clone https://github.com/Rafael-Rech/rubiks-cube-2x2x2-ga.git
   ```
2. Execute all cells in the .ipynb file.

---

## Academic Context

This project was created as part of the **Natural Computing** subject, aiming to demonstrate:

* Application of evolutionary algorithms
* Encoding strategies for combinatorial puzzles
* Performance evaluation of heuristic search methods

## The team

This project was done in collaboration with:

- @devLIPEr
- @mprocz