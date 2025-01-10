# F# Mutability Bug
This example demonstrates a common issue in F# related to mutability and unexpected results when modifying mutable variables after a function call. The initial values of `x` and `y` are used in the `add` function, and subsequent modifications to `x` and `y` do not change the already computed value of `z`.

## How to Reproduce
1.  Compile and run `bug.fs`
2. Observe that the output shows the initial sum and not the sum with updated `x` and `y` values.

## Solution
The solution involves understanding F#'s immutability by default and how to address mutable variables correctly for desired behavior.