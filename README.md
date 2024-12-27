# Unexpected Null Behavior in Addition Function

This repository demonstrates a common JavaScript error related to null value handling in functions.  The `foo` function unexpectedly returns `null` if either input is `null`, rather than performing an addition with 0 as a default.

## Bug

The `bug.js` file contains the flawed function.  It uses a strict equality check (`===`) which results in the function short-circuiting and returning `null` when either argument is null. 

## Solution

The `bugSolution.js` file provides a corrected version of the function. The solution uses loose equality (`==`) to handle the null values, which allows the function to proceed even if either input is null.  Alternatively, a more explicit check could have been implemented to treat null values as 0.