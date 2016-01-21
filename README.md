hsudoku is a sudoku solver written in Haskell.

When I studied functional programming at the university we got to write
a sudoku solver in Haskell by using backtracking. Now that is not especially
efficient, and it does not represent how humans think about sudokus.

Nowadays, I don't get to do any Haskell at work, so this is mostly just to
make sure I won't forget anything, and a neat way to solve sudokus by using
the same techniques humans do.


How to run
----------
You'll need a Haskell compiler and/or interpreter. 

To run compiled:
```
$ ghc -O2 -o hsudoku
$ ./hsudoku "test.sud"
```

To run interpreted:
```
$ ghci Solve.hs
*Solve> sud <- readSudoku "test.sud"
*Solve> putStrLn $ printBoard $ solve sud
```
