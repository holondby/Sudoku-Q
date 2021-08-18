# Sudoku-Q

The Sudoku-Q algorithm solves standard Sudoku puzzles of any complexity (so far at least). The algorithm uses q-learning to generate its solution. Convergence on a solution is often suprisingly rapid. For the 40 puzzles explored, the Sudoku-Q Notebook documents the number of learning trials required for convergence.  All 40 of the puzzles discussed, as well as the 'test.txt' dataset discused in the Notebook, are found in the Datasets folder.

The ltm.npy file is the stored long term memory that results when all 40 puzzles are trained using the same memory. When the ltm.npy file is specified as the memory_file in the Sudoku-Q main() function, running any of the 40 puzzles will recall the correct (greedy q-value driven) solution path. The hope is that, when trained on enough puzzles, the algorithm will learn to generalize. So far, this has not been achieved. The question of generalization, as well as a number of other potential areas of research, are discussed in the Sudoku-Q Notebook.

>Note To train an empty (i.e. *tabula rasa*) memory, simply change the memory_file name, in the Sudoku-Q main() function, to some non-existing file name.

The Print_Dictionary application displays the contents of the dictionary. It should be used with care, however, when run against a large memory, the program can generate substantial screen output.
