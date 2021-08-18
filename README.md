# Sudoku-Q

The Sudoku-Q algorithm solves standard Sudoku puzzles of any complexity (so far at least). The algorithm uses q-learning to generate its solution. Convergence on a solution is often suprisingly rapid. For the 40 puzzles explored, the Sudoku-Q Notebook documents the number of learning trials required for convergence.  All 40 of the puzzles discussed, as well as the 'test.txt' dataset discused in the Notebook, are found in the Datasets folder.

When all 40 puzzles are trained against the same memory or memory_file, re-running any of the puzzles recalls the correct (greedy q-value driven) solution path. The hope is that when the algorithm is trained on enough puzzles, potential intermediate state interactions will eventually lead to generalization. This has not, as yet, been achieved. The issue of generalization, as well as other potential areas of research, are discussed in the Sudoku-Q Notebook.

>Note To train an empty (i.e. *tabula rasa*) memory, simply change the memory_file name in the Sudoku-Q main() function, to some non-existing .npy file name.

The Print_Dictionary application displays the contents of the dictionary. It should be used with care, however. When run against a large memory, the program can generate substantial screen output.
