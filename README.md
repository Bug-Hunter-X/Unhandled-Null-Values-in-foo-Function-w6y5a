# Unhandled Null Values in foo Function

This repository demonstrates a common JavaScript error: unexpected null values not being handled properly in a function. The `foo` function is designed to perform an operation, but it does not explicitly check for null values as input, which can lead to errors or unexpected behavior.

## Bug Description
The `foo` function does not handle null input values correctly. When passed null values for `a` or `b`, it will throw an error.  This is a common issue when interacting with external data sources or when dealing with optional parameters.

## Solution
The solution involves adding a check at the beginning of the function to explicitly handle null values. If either `a` or `b` is null, the function returns null, preventing unexpected errors.

## How to reproduce the bug
1. Clone the repository.
2. Open `bug.js` in a JavaScript environment and run the `foo` function with different values, including null.
3. Observe the output and the error when null is used.

## How to fix the bug
1. Open `bugSolution.js`. Observe the added condition to handle null input values.
2. Run the `foo` function from the `bugSolution.js` file with different values including null.
3. Verify that the function now correctly handles null values and returns null without errors.