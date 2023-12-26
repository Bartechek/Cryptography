# Cryptography
Encrypt and decrypt data using the Cryptography library.
from cryptography.fernet import Fernet

# Generate a key
key = Fernet.generate_key()
cipher_suite = Fernet(key)

# Encrypt data
data = b"Hello, this is a secret message."
cipher_text = cipher_suite.encrypt(data)

# Decrypt data
decrypted_data = cipher_suite.decrypt(cipher_text)
