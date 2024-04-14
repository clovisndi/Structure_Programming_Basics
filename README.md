# Structure_programming_Basics/power.c
Here, the `pow_recursion` function is defined recursively, where if the exponent `y` is negative, the function returns -1, if it is 0, the function returns 1, and if it is greater than 0, the function multiplies the base `x` to the result of `x` raised to the exponent `y-1`.

In `main()`, the user inputs the base `x` and the exponent `y`, which are then used to call the `pow_recursion` function and output the result using `printf`.

Note: In the original code, there was a missing semicolon at the end of the `return` statement in `main()`. This has been corrected in the updated code.
