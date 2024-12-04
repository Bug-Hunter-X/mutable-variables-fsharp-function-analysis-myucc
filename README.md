# F# Mutable Variable Bug

This example demonstrates unexpected behavior when using mutable variables within a function in F#. The `add` function aims to add two mutable variables, but the result is not what's expected due to how the mutable assignments interact.

## Problem

The code uses mutable variables (`x` and `y`) and modifies them within the `add` function. The unexpected result arises from how these modifications affect the subsequent calculations.

## Solution

The solution shows how to achieve the intended behavior while working around the unexpected behavior of mutable variables by using local variables within the function instead. This prevents interference between mutable variables across different parts of the function call.