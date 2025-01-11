# Unexpected Behavior with Null Parameters in JavaScript Function

This repository demonstrates a subtle bug in a JavaScript function that handles null parameters unexpectedly. The function `foo` is intended to add two numbers, but it returns 0 if either parameter is null. This behavior may not be immediately obvious and could lead to unexpected results in applications using this function.

## Bug Description

The bug lies in the function's handling of null parameters.  Instead of treating null as 0, the function returns 0 immediately when it encounters a null parameter. This differs from the expected behavior, which might involve treating null parameters as 0 before performing the addition.

## Solution

The solution involves explicitly handling null values by converting them to 0 before performing the addition. This ensures that the function behaves as expected, even when null values are passed as arguments.

## How to Reproduce

1. Clone this repository.
2. Open `bug.js` to see the buggy implementation.
3. Run the code in a JavaScript environment. Observe the unexpected results.
4. Examine `bugSolution.js` to see the corrected code and its improved behavior.