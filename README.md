# Encryption-program
Encryption program in Python 🔒
import random
import string

chars = " " + string.punctuation + string.digits + string.ascii_letters

chars = list(chars)
key = chars.copy() 

random.shuffle(key)
# ENCRYPTION

plan_text  = input("Enter a message to encrypt: ")
cipher_text = ""

for letter in plan_text:
    index = chars.index(letter)
    cipher_text += key[index]

print(f"Original message : {plan_text}")
print(f"encrypted message: {cipher_text}"

# DECRYPTION
cipher_text  = input("Enter a message to encrypt: ")
plan_text = ""

for letter in cipher_text:
    index = key.index(letter)
    plan_text += chars[index]

print(f"encrypted message: {plan_text}")
print(f"Original message : {cipher_text}")
