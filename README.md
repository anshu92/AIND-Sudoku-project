# Artificial Intelligence Nanodegree
## Introductory Project: Diagonal Sudoku Solver

# Question 1 (Naked Twins)
Q: How do we use constraint propagation to solve the naked twins problem?  
A: In the naked twin problem, the constraint that occurs is that two boxes within a unit can contain the same character space of size 2. That is, within that unit, those two characters can only occur in those two boxes. This means that all other boxes in that unit cannot contain those characters. And hence by 'propagating' this local constraint to the other boxes in the unit, we can safely eliminate the two characters as possibilities in the other boxes.

# Question 2 (Diagonal Sudoku)
Q: How do we use constraint propagation to solve the diagonal sudoku problem?  
A: The constraint in this case is that the numbers 1-9 can occur only once across the two diagonals in a sudoku puzzle. And so, by adding this constraint as we perform the strategies of elimination, one choice and search, we are reducing the space of possible values in some boxes by adding the rule that if the number has already occured in the diagnal, it cannot occur in the box in consideration.

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