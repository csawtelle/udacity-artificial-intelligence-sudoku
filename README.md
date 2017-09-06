# Artificial Intelligence Nanodegree
## Introductory Project: Diagonal Sudoku Solver

# Question 1 (Naked Twins)
Q: How do we use constraint propagation to solve the naked twins problem?

A: In this exercise we used the common constraints of Sudoku to make an assumptions about a boxes value. This is the usual way that a human would solve Sudoku, taking it step by step and using the process of elimination to decide which values could potentially go in each box. We used this information to apply an algorithm that stated simply: “If two boxes contain the same two values, then those two boxes will correlate to those two values.” Even though we don’t know which box is which, we can eliminate those two values from the rest of the units. This applies an additional constraint to the system that helps us reduce the search space.

# Question 2 (Diagonal Sudoku)
Q: How do we use constraint propagation to solve the diagonal Sudoku problem?

A: In order to solve a Sudoku puzzle, each "unit" is constrained by a certain set of rules. In this case we make sure that each row, column, and 3x3 square contains only
the numbers 1-9 uniquely within itself. After providing the standard units for Sudoku, an additional two units were added to represent the diagonals.

### Install

This project requires **Python 3**.

We recommend students install [Anaconda](https://www.continuum.io/downloads), a pre-packaged Python distribution that contains all of the necessary libraries and software for this project. 
Please try using the environment we provided in the Anaconda lesson of the Nanodegree.

##### Optional: Pygame

Optionally, you can also install pygame if you want to see your visualization. If you've followed our instructions for setting up our conda environment, you should be all set.

If not, please see how to download pygame [here](http://www.pygame.org/download.shtml).

### Code

* `solution.py` - You'll fill this in as part of your solution.
* `solution_test.py` - Do not modify this. You can test your solution by running `python solution_test.py`.
* `PySudoku.py` - Do not modify this. This is code for visualizing your solution.
* `visualize.py` - Do not modify this. This is code for visualizing your solution.

### Visualizing

To visualize your solution, please only assign values to the values_dict using the `assign_value` function provided in solution.py

### Submission
Before submitting your solution to a reviewer, you are required to submit your project to Udacity's Project Assistant, which will provide some initial feedback.  

The setup is simple.  If you have not installed the client tool already, then you may do so with the command `pip install udacity-pa`.  

To submit your code to the project assistant, run `udacity submit` from within the top-level directory of this project.  You will be prompted for a username and password.  If you login using google or facebook, visit [this link](https://project-assistant.udacity.com/auth_tokens/jwt_login) for alternate login instructions.

This process will create a zipfile in your top-level directory named sudoku-<id>.zip.  This is the file that you should submit to the Udacity reviews system.

