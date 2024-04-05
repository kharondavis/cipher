# Vigenère Cipher

The Vigenère cipher is a method of encrypting alphabetic text using a simple form of polyalphabetic substitution. This Python implementation demonstrates how the Vigenère cipher algorithm encrypts and decrypts messages.

## How It Works

The Vigenère cipher works by shifting each letter of the plaintext message according to a repeating keyword. The encryption and decryption processes involve finding the offset for each letter in the keyword and shifting the corresponding plaintext letter accordingly.

The following functions are used in this implementation:

- `vigenere(message, key, direction=1)`: This function performs the Vigenère cipher encryption and decryption. It takes three arguments: `message` (the plaintext message to encrypt or decrypt), `key` (the encryption key), and `direction` (optional, specifies whether to encrypt or decrypt the message).
- `encrypt(message, key)`: This function encrypts a plaintext message using the Vigenère cipher with the specified encryption key.
- `decrypt(message, key)`: This function decrypts an encrypted message using the Vigenère cipher with the specified decryption key.

## Example

Here's an example of how the Vigenère cipher is used to encrypt and decrypt a message:

```python
# Example usage
text = "Hello, World!"
custom_key = "KEY"

# Encrypt the message
encrypted_text = encrypt(text, custom_key)
print("Encrypted text:", encrypted_text)

# Decrypt the encrypted message
decrypted_text = decrypt(encrypted_text, custom_key)
print("Decrypted text:", decrypted_text)
```
In the example above, the plaintext message "Hello, World!" is encrypted using the encryption key "KEY". The encrypted text is then decrypted using the same decryption key, resulting in the original plaintext message.

## Note
This implementation is provided for educational purposes to demonstrate how the Vigenère cipher works. It is not intended for production use and may not provide strong encryption.


