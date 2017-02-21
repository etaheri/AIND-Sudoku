# Artificial Intelligence Nanodegree
## Introductory Project: Diagonal Sudoku Solver

# Question 1 (Naked Twins)
Q: How do we use constraint propagation to solve the naked twins problem?  
A: Constraint propagation is used to solve the naked twins project by adding another process to our sudoku puzzle solution. By adding naked twins we have introduced another way of reducing our puzzle. We know that if two boxes in the same unit share the same two possible digits, the remaining boxes in the unit cannot contain those values. We can now solve the puzzle by repeating elimination, only-choice, and naked twins until the puzzle is complete.

# Question 2 (Diagonal Sudoku)
Q: How do we use constraint propagation to solve the diagonal sudoku problem?  
A: We can use constraint propagation to solve the diagonal sudoku by using the same constraints from the traditional sudoku, but add the additional rules for the two diagonal units. We already account for the row, column, and square units. The solution is to add units for the diagonal sections and append those units to the list off all units. When reducing the puzzle, the elimination and only choice steps will account for the new constraints in determining the solution. 

### Install

This project requires **Python 3**.

We recommend students install [Anaconda](https://www.continuum.io/downloads), a pre-packaged Python distribution that contains all of the necessary libraries and software for this project. 
Please try using the environment we provided in the Anaconda lesson of the Nanodegree.

##### Optional: Pygame

Optionally, you can also install pygame if you want to see your visualization. If you've followed our instructions for setting up our conda environment, you should be all set.

If not, please see how to download pygame [here](http://www.pygame.org/download.shtml).

### Code

* `solutions.py` - You'll fill this in as part of your solution.
* `solution_test.py` - Do not modify this. You can test your solution by running `python solution_test.py`.
* `PySudoku.py` - Do not modify this. This is code for visualizing your solution.
* `visualize.py` - Do not modify this. This is code for visualizing your solution.

### Visualizing

To visualize your solution, please only assign values to the values_dict using the ```assign_values``` function provided in solution.py

### Data

The data consists of a text file of diagonal sudokus for you to solve.
