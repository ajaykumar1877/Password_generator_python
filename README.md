import random
import string

def generate_password():
    # Prompt user to specify the desired length of the password
    length = int(input("Enter the desired password length: "))

    # Define characters to be used for the password
    characters = string.ascii_letters + string.digits + string.punctuation

    # Generate a random password using the specified length
    password = ''.join(random.choice(characters) for i in range(length))

    # Display the generated password
    print(f"Generated Password: {password}")

# Call the function to generate the password
generate_password()
