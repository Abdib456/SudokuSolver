# SudokuSolver
This is my sudoku solver program.

My code uses a combination of constraint satisfaction and backtracking techniques to solve these sudokus.

My functions:
1)'find_empty_location': Returns row and column of the empty cels or None if the board is full

2)'is_valid': Checks if number is allowed to be placed in a given cell. It returns true if valid and false if not.

3)'apply_constraint': Does the constraint satisfaction so it narrows down the possible values that can be put in a empty cell. It does this by checking values in the same row, column and 3x3 box and removing the values it can't be from the set of numbers. This process is repeated till no more updates to the board can be made.

4)'solved_sudoku': Does the backtracking algorithm. It does this by trying is possible value for a cell and it keeps going until it can't find one if so it backtracks and starts again.

5)'check_board': Does the final check of the board to see if there is any numbers which are in the wrong spaces in order to make sure an incorrect sudoku isn't the output.

6)'sudoku solver': The main function which outputs the solved sudoku or the sudoku filled with -1s when there is no solution.


Reducing time complexity:
The constraint satisfaction was used to reduce the time complexity as it narrows down the possible values that can be put in a empty cell. Backtracking also reduces the time taken as it doesn't need to explore every possible solution to find the correct answer.
