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

# Structure_programing_Basic/character.c

This is a C program that takes a single character input from the user and determines if it is a capital letter, a small case letter, a digit, or a special symbol. Here's a brief explanation of how it works:

1. The program declares a character variable `c`.

2. The user is prompted to enter a character. The character is read into `c` using the `scanf` function.

3. The program then uses a series of `if-else` statements to check whether the character is a capital letter, a small case letter, a digit, or a special symbol. If the character falls into any of these categories, a corresponding message is printed using `printf`.

4. The `main` function returns 0 to indicate successful execution.

# Structure_Programming_Basics/problem1.c

Sure, let me explain this code line by line:

1. `#include <stdio.h>`: This line includes the standard input-output library in the program.

2. `int main() {`: This line marks the beginning of the program's main function.

3. `float balance, annualInterestRate, monthlyPaymentRate;`: This line declares three float variables to store the credit card balance, annual interest rate and minimum monthly payment rate, respectively.

4. `printf("Enter the outstanding balance on the credit card: ");`: This line prints a message prompting the user to enter the outstanding balance on the credit card.

5. `scanf("%f", &balance);`: This line reads the balance entered by the user and stores it in the `balance` variable.

6. `printf("Enter the annual interest rate (as a decimal): ");`: This line prints another message prompting the user to enter the annual interest rate.

7. `scanf("%f", &annualInterestRate);`: This line reads the annual interest rate entered by the user and stores it in the `annualInterestRate` variable.

8. `printf("Enter the minimum monthly payment rate (as a decimal): ");`: This line prompts the user to enter the minimum monthly payment rate.

9. `scanf("%f", &monthlyPaymentRate);`: This line reads the minimum monthly payment rate entered by the user and stores it in the `monthlyPaymentRate` variable.

10. `float monthlyInterestRate = annualInterestRate / 12.0;`: This line calculates the monthly interest rate by dividing the annual interest rate by 12 and storing it in the `monthlyInterestRate` variable.

11. `float totalPaid = 0.0;`: This line initializes the `totalPaid` variable to zero, which will be used later to keep track of the total amount paid.

12. `for (int i = 1; i <= 12; i++) {`: This line starts a loop that will iterate 12 times, once for each month of the year.

13. `float minMonthlyPayment = monthlyPaymentRate * balance;`: This line calculates the minimum monthly payment by multiplying the monthly payment rate by the outstanding balance and stores it in `minMonthlyPayment`.

14. `float monthlyUnpaidBalance = balance - minMonthlyPayment;`: This line calculates the monthly unpaid balance by subtracting the minimum monthly payment from the outstanding balance and stores it in `monthlyUnpaidBalance`.

15. `balance = monthlyUnpaidBalance + (monthlyInterestRate * monthlyUnpaidBalance);`: This line updates the outstanding balance by adding the interest accrued on the unpaid balance and subtracting the minimum monthly payment.

16. `totalPaid += minMonthlyPayment;`: This line adds the minimum monthly payment to the `totalPaid` variable.

17. `printf("Month: %d\n", i);`: This line prints the current month number.

18. `printf("Minimum monthly payment: %.2f\n", minMonthlyPayment);`: This line prints the minimum monthly payment with two decimal places.

19. `printf("Remaining balance: %.2f\n", balance);`: This line prints the remaining balance after paying the minimum monthly payment with two decimal places.

20. `}`: This line marks the end of the loop.

21. `printf("Total paid: %.2f\n", totalPaid);`: This line prints the total amount paid with two decimal places.

22. `printf("Remaining balance: %.2f\n", balance);`: This line prints the remaining balance after one year with two decimal places.

23. `return 0;`: This line marks the end of the program, and returns 0 to indicate the successful termination of the program.


# Structure_Programming_Basics/magical_number.c

This program takes a three-digit integer input from the user, checks if it is a "magic number" (i.e., a palindrome), and outputs a message indicating whether or not it is.

The important lines of code include:

1. Lines 3-4 declare the variables `num` and `reversed` as integers, and `originalNum` as an integer that stores the original input value.

2. Lines 6-7 prompt the user to enter a three-digit integer, and read the input value into the `num` variable.

3. Lines 10-14 use an if statement to check that the input value is positive and has exactly three-digits. If either of these conditions is not met, the program prints an error message and returns a status code of 1, indicating a failure to execute the program.

4. Line 16 stores the original input value in the `originalNum` variable for output.

5. Lines 19-23 use a while loop to reverse the `num` variable. `reversed` is first multiplied by 10 and then added to `num % 10` (the ones digit of `num`). Finally, `num` is updated to remove the last digit by dividing by 10.

6. Lines 26-29 use an if statement to check if the reversed value `reversed` is equal to the original value `originalNum`. If they are equal, the program prints a message indicating that the input is a "magic number". If they are not equal, the program prints a message indicating that the input is not a "magic number".

7. Line 31 returns 0 to indicate successful execution of the program.

Overall, this program takes a three-digit integer input from the user, checks that it is a valid input (positive and three-digit), checks if it is a palindrome or "magic number", and outputs an appropriate message to the console indicating the result.

# Sructure_Programming_Basics/Problem2.c





