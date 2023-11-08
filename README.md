# Password Checker

This Python script checks the security of your passwords by querying the "Have I Been Pwned" API. It helps you determine if a password has been exposed in a data breach.

## How it works
- The script takes one or more passwords as input.
- It converts each password into a SHA-1 hash and sends the first five characters of the hash to the "Have I Been Pwned" API.
- The API returns a list of suffixes of SHA-1 hashes of compromised passwords that match the first five characters.
- The script checks if the rest of the hash of the password is present in the list of compromised passwords.
- If a match is found, it means the password has been exposed in a data breach.

## Usage
1. Clone this repository or download the script.
2. Run the script with one or more passwords as arguments.
   ```bash
   python password_checker.py password1 password2
