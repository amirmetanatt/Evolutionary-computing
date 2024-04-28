
# Genetic Algorithm for boiler Optimization Problem

This code implements a genetic algorithm to solve an optimization problem with constraints. The genetic algorithm is used to find the optimal solution to the problem by evolving a population of individuals over multiple generations.

## Problem Description

The optimization problem is defined with the following constraints:

- Four variables: x[0], x[1], x[2], x[3]
- Constraints on variables:
  - 0 <= x[0] <= 100
  - 0 <= x[1] <= 100
  - 10 <= x[2] <= 200
  - 10 <= x[3] <= 200
- Objective function to minimize:
  - 0.6224 * x[0] * x[2] * x[3] + 1.7781 * x[1] * x[2]^2 + 3.1661 * x[0]^2 * x[3] + 19.84 * x[0]^2 * x[2] + penalty
- Constraints:
  - -x[0] + 0.0193 * x[2] <= 0
  - -x[1] + 0.00954 * x[2] <= 0
  - -π * x[2]^2 * x[3] - (4/3) * π * x[2]^3 + 1296000 <= 0
  - x[3] - 240 <= 0
  - Variable lower bounds: -x[0], -x[1], -x[2] + 10, -x[3] + 10
  - Variable upper bounds: x[0] - 100, x[1] - 100, x[2] - 200, x[3] - 200

## Installation

Make sure you have Python 3.x installed. You can install the required dependencies using pip:

```bash
pip install numpy matplotlib
```

## Usage

To run the genetic algorithm, execute the following command:

```bash
python genetic_algorithm.py
```

The algorithm will evolve a population of individuals over multiple generations and output the best solution found along with a fitness curve showing the evolution of the best fitness value over generations.




## Boiler Mathematical Formulation


![BoilerMath(project2)](https://github.com/amirmetanatt/Evolutionary-computing/assets/147061622/cd3aad40-cbe2-47b6-b7f0-7b11a17e6a66)

## Notes
Ensure you have all the required libraries installed before running the projects.
Modify the parameters in the code for different experimentations.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
