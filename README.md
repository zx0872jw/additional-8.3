# additional-8.3
# write def encrypt(user_input, encryption_library, decryption_library)
def encrypt(user_input, encryption_library, decryption_library)
    new_input = user_input.translate(encryption_library)
    print(new_input)
    print(new_input.translate(decryption_library))
    
    
def main():
    user_input = input("Enter a sentence: ")
    encryption_library = str.maketrans("ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz", "1234567890-=!@#$%^&*()_+[]jklmnopqrstuvwxyzabcdefghi")
    decryption_library = str.maketrans("1234567890-=!@#$%^&*()_+[]jklmnopqrstuvwxyzabcdefghi", "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz")
    
    encrypt(user_input, encryption_library, decryption_library)
