Password Strength and Leak Checker

Overview:

This project checks whether a password has appeared in known data breaches and evaluates its basic strength.
It uses the Have I Been Pwned (HIBP) Pwned Passwords API.

Features:

Checks passwords against known leaked passwords.
Uses SHA-1 hashing and the first five hash characters for a k-anonymity lookup.
Reports the number of known exposures.
Checks password length, uppercase letters, numbers, and symbols.
Classifies passwords as Very Weak, Weak, Medium, or Strong.

Requirements:

Python 3.8 or newer
Internet connection
requests package
Install the dependency:
pip install -r requirements.txt

How to Run:

Save the Python code as password_checker.py, then run:
python password_checker.py
You can also run it directly in Thonny.


How It Works:

The password is converted into an uppercase SHA-1 hash.
Only the first five characters of the hash are sent to the HIBP API.
The returned hash suffixes are checked locally.
If a match is found, the program reports the leak count.
Otherwise, the program checks length and character types.

Privacy and Security:

The complete password and complete hash are not sent to the API. Only the first five hash characters are sent using the k-anonymity approach.
This is an educational project. Do not print, log, or share real passwords. The strength rules used here are basic and are not a complete password-security assessment.


