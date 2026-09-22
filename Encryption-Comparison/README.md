Encryption Comparison Project

Overview:

This project compares three encryption methods:
Caesar Cipher
Vigenère Cipher
AES-256-GCM

The program encrypts and decrypts text with each method and verifies that the decrypted text matches the original message.

Features:

Caesar cipher encryption and decryption
Vigenère cipher encryption and decryption
AES-256-GCM encryption and decryption
Base64 encoding for AES output
Decryption verification
Interactive menu

Requirements:

Python 3.8 or newer
cryptography
Install the dependency:
pip install -r requirements.txt

How to Run:

Open the Python file in Thonny.
Install the required dependency.
Run the program.
Follow the menu instructions.

Security Note:

Caesar and Vigenère are classical educational ciphers and should not be used to protect sensitive information.
AES-256-GCM provides encryption and authentication. Keep the AES key secret and do not reuse a nonce with the same key.

Verification:

The program compares each decrypted message with the original plaintext. True means the result was successfully recovered.
