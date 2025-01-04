# Incorrect Number Comparison in TypeScript Sorting Function

This repository demonstrates a common bug in TypeScript: an incorrect comparison function used for sorting numbers. The `compare` function, as initially written, uses simple subtraction (`a - b`), which leads to incorrect results when dealing with negative numbers. This bug manifests when attempting to sort an array containing both positive and negative numbers.

## Bug Description
The subtraction method (`a - b`) in the `compare` function will not sort negative numbers correctly.  For example, comparing -5 and -2 will result in -3, causing -5 to appear before -2 in the sorted array, which is incorrect.