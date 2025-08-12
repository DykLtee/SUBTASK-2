# SUBTASK-2
def decimal_to_binary(n):
    return bin(n)[2:]

def binary_to_decimal(b):
    return int(b, 2)

def decimal_to_hexadecimal(n):
    return hex(n)[2:]

def hexadecimal_to_decimal(h):
    return int(h, 16)

def main():
    while True:
        print("Menu:")
        print("1. Convert Decimal to Binary")
        print("2. Convert Binary to Decimal")
        print("3. Convert Decimal to Hexadecimal")
        print("4. Convert Hexadecimal to Decimal")
        print("5. Quit")
        
        choice = input("Enter your choice: ")
        
        if choice == "1":
            num = int(input("Enter a decimal number: "))
            print(f"The binary equivalent of {num} is {decimal_to_binary(num)}")
        elif choice == "2":
            num = input("Enter a binary number: ")
            print(f"The decimal equivalent of {num} is {binary_to_decimal(num)}")
        elif choice == "3":
            num = int(input("Enter a decimal number: "))
            print(f"The hexadecimal equivalent of {num} is {decimal_to_hexadecimal(num)}")
        elif choice == "4":
            num = input("Enter a hexadecimal number: ")
            print(f"The decimal equivalent of {num} is {hexadecimal_to_decimal(num)}")
        elif choice == "5":
            break
        else:
            print("Invalid choice. Please try again.")

if _name_ == "_main_":
    main()
