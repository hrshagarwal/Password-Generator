# Password Generator

This project generates a secure, random password based on user-defined constraints such as minimum numbers, special characters, uppercase and lowercase letters.<br>
It uses Python's `secrets` module for cryptographically strong randomness.<br><br>

## Features
- Generate passwords of customizable length (default 16 characters).<br>
- Ensure minimum numbers, special characters, uppercase and lowercase letters.<br>
- Uses regex to verify the presence of required character types.<br><br>

## How It Works

The program generates random passwords from a combined set of characters:<br>
- Letters (both uppercase and lowercase)<br>
- Digits<br>
- Special symbols (punctuation)<br><br>

After generating a password, it uses **regular expressions (regex)** to check if the password meets all constraints.<br>
Regular expressions are patterns used to match specific character sets in strings.<br>
For example:<br>
- `\d` matches any digit<br>
- `[A-Z]` matches any uppercase letter<br>
- `[a-z]` matches any lowercase letter<br>
- `[!@#$%^&*]` matches specific special characters<br><br>

The program repeats generating passwords until it finds one that satisfies all rules.<br><br>

## Usage

Simply run the script:<br>
```bash
python generate_password.py
