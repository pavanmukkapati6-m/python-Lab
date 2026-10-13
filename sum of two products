def input_matrix(rows, cols, name):
    print(f"\nEnter elements of Matrix {name} ({rows}x{cols}):")
    matrix = []

    for i in range(rows):
        while True:
            raw_input = input(f"Row {i+1}: ").strip().split()
            if len(raw_input) != cols:
                print(f"Invalid row length. Please enter exactly {cols} values.")
                continue

            try:
                row = [int(val) for val in raw_input]
                matrix.append(row)
                break
            except ValueError:
                print("Invalid input. Please enter integers only for this row.")

    return matrix


def add_matrices(A, B):
    return [[A[i][j] + B[i][j] for j in range(len(A[0]))] for i in range(len(A))]


def multiply_matrices(A, B):
    result = []
    for i in range(len(A)):
        row = []
        for j in range(len(B[0])):
            product = sum(A[i][k] * B[k][j] for k in range(len(B)))
            row.append(product)
        result.append(row)
    return result


def main():
    try:
        r1 = int(input("Enter number of rows for Matrix A: "))
        c1 = int(input("Enter number of columns for Matrix A: "))
        r2 = int(input("Enter number of rows for Matrix B: "))
        c2 = int(input("Enter number of columns for Matrix B: "))

        if min(r1, c1, r2, c2) <= 0:
            print("Error: Matrix dimensions must be positive integers.")
            return

        A = input_matrix(r1, c1, "A")
        B = input_matrix(r2, c2, "B")

        if r1 == r2 and c1 == c2:
            print("\nMatrix Addition (A + B):")
            for row in add_matrices(A, B):
                print(row)
        else:
            print("\nMatrix addition not possible (incompatible dimensions).")

        if c1 == r2:
            print("\nMatrix Multiplication (A x B):")
            for row in multiply_matrices(A, B):
                print(row)
        else:
            print(
                "\nMatrix multiplication not possible (Columns of A must equal rows of B)."
            )

    except ValueError:
        print("Invalid input. Please enter valid integers for matrix dimensions.")


if __name__ == "__main__":
    main()