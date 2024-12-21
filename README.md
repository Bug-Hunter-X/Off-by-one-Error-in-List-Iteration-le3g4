# Off-by-one Error in Dart List Iteration

This repository demonstrates a common off-by-one error in Dart when iterating over a list using a `for` loop.  The error occurs when the loop condition `i <= numbers.length` attempts to access an index that is out of bounds for the list.

## Bug
The `bug.dart` file contains the erroneous code.  The loop attempts to access `numbers[numbers.length]`, which results in an `RangeError` exception.

## Solution
The `bugSolution.dart` file provides a corrected version. The loop condition is changed to `i < numbers.length`, preventing the out-of-bounds access.

This example highlights the importance of carefully considering loop conditions when working with lists or arrays in Dart.