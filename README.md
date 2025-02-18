# Unexpected TypeError when accessing object properties in JavaScript

This example demonstrates a common JavaScript error: `TypeError: Cannot read properties of undefined (reading 'length')`. This occurs when attempting to access a property (in this case, `length`) of an object that is either `null` or `undefined`.

The `bug.js` file contains code that incorrectly handles these cases, leading to the error. The `bugSolution.js` file shows the corrected version.

## How to reproduce

1.  Clone this repository.
2.  Run `node bug.js`.
3.  Observe the `TypeError`.
4.  Run `node bugSolution.js` to see the corrected behavior.

## Solutions

The solution involves explicitly checking for `null` or `undefined` before attempting to access object properties.  The best approach is to use optional chaining (`?.`) and nullish coalescing (`??`) operators introduced in ES2020. These offer concise and readable solutions.

If you're using older JavaScript versions, the traditional `if` statement still works effectively.