# Solve Sudoku with AI

## Synopsis

In this project, you will extend the Sudoku-solving agent developed in the classroom lectures to solve _diagonal_ Sudoku puzzles and implement a new constraint strategy called "naked twins". A diagonal Sudoku puzzle is identical to traditional Sudoku puzzles with the added constraint that the boxes on the two main diagonals of the board must also contain the digits 1-9 in each cell (just like the rows, columns, and 3x3 blocks). The naked twins strategy says that if you have two or more unallocated boxes in a unit and there are only two digits that can go in those two boxes, then those two digits can be eliminated from the possible assignments of all other boxes in the same unit.


## Quickstart Guide

1. Configure the Environment from aind-universal-v4.yml and activate your python env
   1. `activate aind` - Windows
   2. `$ source activate aind` - Mac/OS X
    
    

2. You can run a small set of test cases using the local test suite. 

    `(aind)$ python -m unittest -v`

3.  You can run the code with visualization (see the last section of the readme for more information)

    `(aind)$ python solution.py`

## Visualization

**Note:** The `pygame` library is required to visualize the sudoku -- however, the `pygame` module can be troublesome to install and configure. It should be installed by default with the AIND conda environment, but it is not reliable across all operating systems or versions. Please refer to the pygame documentation [here](http://www.pygame.org/download.shtml), or discuss among your peers in the slack group if you need help.

Running `python solution.py` will automatically attempt to visualize your solution, but you mustuse the provided `assign_value` function (defined in `utils.py`) to track the puzzle solution progress for reconstruction during visuzalization.
