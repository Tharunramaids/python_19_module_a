# Factorial Program

## Aim
The aim of this program is to calculate the factorial of a given non-negative integer n. The factorial of a number n (denoted n!) is the product of all positive integers less than or equal to n.

## Algorithm
Check for Negative Input:

If n is negative, factorial is not defined; display an appropriate message.

Base Case:

If n is 0 or 1, return 1 (since 0! = 1! = 1).

Recursive Case:

For n > 1, compute faci(n) = n * faci(n - 1) recursively.

## Program
```
def faci(n):
    if n == 0 or n == 1:
        return 1
    else:
        return n * faci(n - 1)

if __name__ == "__main__":
    try:
        n = int(input("Enter a number: "))
    except ValueError:
        print("Please enter a valid integer.")
        exit(1)

    if n < 0:
        print("Factorial is not defined for negative numbers")
    else:
        print(f"Factorial of number {n} = {faci(n)}")
```
## output
![Screenshot 2025-04-29 141801](https://github.com/user-attachments/assets/ba3c7ad5-7a00-4e7e-8e52-6303ad723f1a)

## Result
For valid non-negative inputs, the program outputs the correct factorial value.
For negative inputs, the program gracefully informs the user that factorial is not defined.
