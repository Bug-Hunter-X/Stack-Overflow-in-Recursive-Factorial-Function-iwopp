# Hack Bug Report: Stack Overflow in Recursive Factorial Function

This repository demonstrates a stack overflow error in Hack caused by excessive recursion in a factorial function.  The `bug.hack` file contains the buggy code, which uses recursion to calculate the factorial. For large inputs, this will result in a stack overflow. The `bugSolution.hack` file shows how to fix the issue by using iteration instead of recursion.

## How to reproduce

1. Clone this repository.
2. Compile and run `bug.hack`.  You will observe a stack overflow error if you call foo with a relatively large input.
3. Compile and run `bugSolution.hack`. This version will calculate the factorial correctly without causing a stack overflow.

## Discussion

This bug highlights the importance of considering the limits of the call stack when using recursive functions, especially in Hack which has similar limitations to other languages when dealing with deep recursion.