# Python Password Generator

A simple, interactive command-line utility written in Python that generates strong, customizable, and random passwords. 

## Features
* **Customizable Length:** Define the exact minimum length required for your password.
* **Character Toggles:** Choose whether to include numbers and/or special characters.
* **Guaranteed Complexity:** The algorithm ensures that if you request numbers or special characters, at least one of each will be included in the final password.
* **Input Validation:** Prevents crashes by validating user input for the password length.

## Prerequisites
* Python 3.x installed on your machine.
* No external libraries are required (uses Python's built-in `random` and `string` modules).

## Usage

1. Clone or download the repository to your local machine.
2. Save the code in a file named `password_generator.py`.
3. Open your terminal or command prompt.
4. Navigate to the directory where the file is saved.
5. Run the script using Python:

```bash
python password_generator.py
```

6. Follow the on-screen prompts to generate your password.

## Example

```text
Enter the minimum length of the password: 16
Do you want to have numbers (y/n)? y
Do you want to have special characters (y/n)? y
This is the generated password:  aB3$kL9#mP2!qR5*
```

## How It Works
The script uses a `while` loop to randomly select characters from a predefined pool of letters, numbers (optional), and punctuation marks (optional). It continues adding characters until the password reaches the specified minimum length **and** successfully meets the user's requested character criteria.
