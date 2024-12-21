# JavaScript Loose Comparison Pitfalls with null and undefined

This repository demonstrates a common JavaScript error related to loose comparison (==) when handling null and undefined values.

## The Problem

JavaScript's loose equality operator (==) does not always behave as expected when comparing null and undefined. This can lead to unexpected results and bugs in your code.

The `bug.js` file contains a function that attempts to handle null and undefined values using loose comparison.  However, the result for undefined is unexpected due to type coercion involved in loose comparison.

## The Solution

The `bugSolution.js` file shows the corrected version of the function. This version uses strict equality (===) to explicitly check for null and undefined separately, preventing type coercion and ensuring the expected behavior.

## How to Reproduce

1. Clone this repository.
2. Navigate to the repository's directory.
3. Run `node bug.js` to see the unexpected behavior.
4. Run `node bugSolution.js` to see the corrected behavior.

This example highlights the importance of using strict equality (===) in JavaScript whenever possible, especially when dealing with null and undefined values, to avoid unexpected type coercion.