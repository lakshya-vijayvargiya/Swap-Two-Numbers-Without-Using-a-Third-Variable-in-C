# Swap-Two-Numbers-Without-Using-a-Third-Variable-in-C
This program takes two integers as input. It swaps their values using arithmetic operations instead of a temporary variable. Finally, it displays the values before and after swapping.


#include <stdio.h>

int main() {   
    int a, b;  // Variables to store two numbers

    // Prompt user to enter two numbers
    printf("Enter two numbers: ");
    scanf("%d %d", &a, &b);

    // Display values before swapping
    printf("Before swapping: a = %d, b = %d\n", a, b);

    // Swap logic without using a third variable
    a = a + b;  // Step 1: Add both numbers
    b = a - b;  // Step 2: Subtract new b from sum to get original a
    a = a - b;  // Step 3: Subtract new b from sum to get original b

    // Display values after swapping
    printf("After swapping: a = %d, b = %d\n", a, b);

    return 0;  // End of program
}
