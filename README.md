# JavaScript Closure Issue in setTimeout Loop

This repository demonstrates a common JavaScript closure issue that arises when using `setTimeout` within a loop.  The problem is that the value of `i` is not captured correctly for each iteration of the loop within the `setTimeout` callbacks.

## Bug

The `bug.js` file contains the buggy code. When executed, it will print the number 10 ten times, instead of printing the numbers 0 through 9 sequentially with a one-second delay.

## Solution

The `bugSolution.js` file demonstrates how to fix this issue using an immediately invoked function expression (IIFE) to create a new scope for each iteration of the loop, thus capturing the correct value of `i` for each callback.