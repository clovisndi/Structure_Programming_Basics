# Structure_programming_Basics/power.c
Here, the `pow_recursion` function is defined recursively, where if the exponent `y` is negative, the function returns -1, if it is 0, the function returns 1, and if it is greater than 0, the function multiplies the base `x` to the result of `x` raised to the exponent `y-1`.

In `main()`, the user inputs the base `x` and the exponent `y`, which are then used to call the `pow_recursion` function and output the result using `printf`.

Note: In the original code, there was a missing semicolon at the end of the `return` statement in `main()`. This has been corrected in the updated code.

# Structure_programming_Basics/Binary_search.c

This program performs a binary search on an integer array provided by the user to find a specific element.

The important lines of code include:

1. Lines 3-12 define the `binarySearch` function that takes the integer array, the starting and ending indices of the search range, and the target element as parameters. The function checks if the ending index is greater than or equal to the starting index, and if so, calculates the middle index and compares the target element with the element at the middle index. If the target element is found, the middle index is returned. Otherwise, the function is called recursively on either the left or right half of the array, depending on whether the target element is less than or greater than the middle element. If the target element is not found in the array, the function returns -1.

2. Lines 14-18 prompt the user to input the size of the integer array and use it to declare the array.

3. Lines 19-23 prompt the user to input the integer values to fill the array.

4. Lines 25-28 prompt the user to input the target element to be searched.

5. Line 30 calls the `binarySearch` function with the integer array, starting index of 0, ending index of size-1, and target element as arguments, and stores the returned index (or -1 if not found) in the `index` variable.

6. Lines 32-35 check if the index is -1 (meaning the element was not found) and prints the appropriate message to the console. Otherwise, it prints the index where the element was found.

# Structure_programing_Basic/
