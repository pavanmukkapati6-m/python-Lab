def read_last_five_lines(filename):
    try:
        with open(filename, "r") as file:
            lines = file.readlines()
            last_five = lines[-5:]

            print("\nLast 5 lines of the file:")
            for line in last_five:
                print(line.strip())

    except FileNotFoundError:
        print(f"Error: file '{filename}' not found.")
    except Exception as e:
        print(f"An error occurred: {e}")

def main():
    filename = input("Enter the filename: ")
    read_last_five_lines(filename)

if __name__ == "__main__":
    main()