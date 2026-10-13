def fibonacci_series(n):
    fib_series = []
    a, b = 0, 1

    for _ in range(n):
        fib_series.append(a)
        a, b = b, a + b

    return fib_series


def main():
    try:
        n = int(input("Enter the number of terms in Fibonacci series: "))

        if n <= 0:
            print("Please enter a positive integer.")
        else:
            result = fibonacci_series(n)
            print(f"Fibonacci series up to {n} terms:")
            print(result)

    except ValueError:
        print("Invalid input. Please enter an integer.")


if __name__ == "__main__":
    main()