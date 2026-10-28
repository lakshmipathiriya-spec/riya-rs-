# Prime Number Checker

This project is a simple Python program that checks whether a given number is a prime number or not.

## What is a prime number?

A prime number is a natural number greater than 1 that has no positive divisors other than 1 and itself.

Examples:
- 2, 3, 5, 7, 11, 13 are prime numbers
- 1, 4, 6, 8, 9, 12 are not prime numbers

## Features
- Accepts a number from the user
- Checks if the number is prime
- Prints a clear result

## Python Code

```python
num = int(input("Enter a number: "))

if num <= 1:
    print(f"{num} is not a prime number.")
elif num == 2:
    print(f"{num} is a prime number.")
else:
    is_prime = True

    for i in range(2, int(num ** 0.5) + 1):
        if num % i == 0:
            is_prime = False
            break

    if is_prime:
        print(f"{num} is a prime number.")
    else:
        print(f"{num} is not a prime number.")
```

## How to Run

1. Open a Python editor or terminal.
2. Save the program in a file, for example `prime_check.py`.
3. Run the script:

```bash
python prime_check.py
```

## Example Output

```bash
Enter a number: 7
7 is a prime number.
```

```bash
Enter a number: 12
12 is not a prime number.
```

## License

This project is open for learning and personal use.
