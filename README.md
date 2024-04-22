import random
import string

def generate_password(length=12):
    # Define characters to choose from
    characters = string.ascii_letters + string.digits + string.punctuation

    # Generate password
    password = ''.join(random.choice(characters) for _ in range(length))
    return password

# Example usage:
generated_password = generate_password()
print("Generated Password:", generated_password)
