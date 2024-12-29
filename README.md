# CSS `calc()` Pitfalls

This repository demonstrates a common issue encountered when using the `calc()` function in CSS: unexpected results due to operator precedence and unit incompatibility.

The `bug.css` file contains the problematic code, while `bugSolution.css` shows the corrected version.

## Problem

Incorrectly using `calc()` can lead to unexpected layout behaviors.  For example, subtracting a unitless number from a percentage can lead to the browser failing to correctly interpret the calculation.

## Solution

Always ensure unit consistency within your `calc()` expressions.  If subtracting or adding values, make sure they have compatible units (e.g., `px`, `em`, `%`, etc.).  Use parentheses to explicitly define operator precedence when needed.