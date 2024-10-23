# Registration Form
def register_user():
    print("Welcome to the Registration Form!")

    # Get user inputs
    name = input("Enter your name: ")
    email = input("Enter your email: ")
    
    # Validating email
    while "@" not in email or "." not in email:
        print("Invalid email format. Please enter a valid email.")
        email = input("Enter your email: ")

    password = input("Enter your password: ")
    confirm_password = input("Confirm your password: ")

    # Password confirmation
    while password != confirm_password:
        print("Passwords do not match. Try again.")
        password = input("Enter your password: ")
        confirm_password = input("Confirm your password: ")

    print("\nRegistration successful!")
    print(f"Name: {name}")
    print(f"Email: {email}")

if __name__ == "__main__":
    register_user()
