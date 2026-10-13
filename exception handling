def divide_numbers(a, b):
    result = None
    try:
        result = a / b
    except ZeroDivisionError:
        print("Error: Division by zero is not allowed.")
    except TypeError:
        print("Error: Please enter only numbers.")
    else:
        print(f"Result of division: {result}")
        return result
    finally:
     print("Execution of divide_numbers() is complete.\n")


def main():
    try:
        x = float(input("Enter the numerator: "))
        y = float(input("Enter the denominator: "))
        divide_numbers(x, y)
    except ValueError:
        print("Error: Invalid input. Please enter numeric values.")


if __name__ == "__main__":
    main()