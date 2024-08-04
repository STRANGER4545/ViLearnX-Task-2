# ViLearnX-Task-2
README
         
    def add(x, y):
        return x + y

    def subtract(x, y):
        return x - y

    def multiply(x, y):
        return x * y

    def divide(x, y):
        if y != 0:
            return x / y
        else:
            return "Error! Division by zero."

    def main():
        print("Welcome to the Simple Calculator!")
    
    # User Input
        try:
            num1 = float(input("Enter the first number: "))
            num2 = float(input("Enter the second number: "))
        except ValueError:
            print("Invalid input! Please enter numeric values.")
            return

    # Operation Selection
        print("\nSelect operation:")
        print("1. Addition")
        print("2. Subtraction")
        print("3. Multiplication")
        print("4. Division")

        choice = input("Enter choice (1/2/3/4): ")

    # Operation Execution and Result Display
        if choice == '1':
            result = add(num1, num2)
            operation = "addition"
        elif choice == '2':
            result = subtract(num1, num2)
            operation = "subtraction"
        elif choice == '3':
        result = multiply(num1, num2)
        operation = "multiplication"
        elif choice == '4':
            result = divide(num1, num2)
            operation = "division"
        else:
            print("Invalid choice! Please select a valid operation.")
            return
    
    # Display Result
        print(f"\nThe result of {operation} between {num1} and {num2} is: {result}")

    if __name__ == "__main__":
        main()
