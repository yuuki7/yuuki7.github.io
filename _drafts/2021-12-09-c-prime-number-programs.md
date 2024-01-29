---
---

Prime number programs can be the first challenge for a beginning programmer.

Definition (Prime number):
An integer n > 1 is prime iff it is not divisible by any integer i such that 2 <= i <= n - 1.

A simple C program to print the primes less than 100 would look like this:

prime.c

    #include <stdio.h>
    
    /**
     * Determines if an integer is prime.
     */
    int is_prime(const int n) {
        int i;
    
        /* Integers less than or equal to 1 are not prime. */
        if (n <= 1) {
            return 0;
        }
    
        /* Performs trial division by every integer `i` such that 2 <= `i` <= `n` - 1. */
        for (i = 2; i < n; i++) {
            if (n % i == 0) {
                return 0;
            }
        }
    
        return 1;
    }
    
    int main(void) {
        int i;
    
        /* Prints the primes less than 100. */
        for (i = 2; i < 100; i++) {
            if (is_prime(i)) {
                printf("%d\n", i);
            }
        }
    
        return 0;
    }

---

    % gcc -Wall -Wextra -o prime prime.c
    % ./prime
    2
    3
    ...
    97
