# LeetCode Notes

This repository contains Jupyter notebooks with coding exercises and their solutions, inspired by and adapted from Reuven M. Lerner's "Python Workout: 50 ten-minute exercises". Below is a summary of the exercises and key skills demonstrated.

## Digital Handling Skills

| Skill | Description | Example |
|-------|-------------|---------|
| User Input | Get user input using input() | `user_guess = input('Guess a number: ')` |
| Integer Conversion | Convert string to integer | `int(user_input)` |
| Random Generation | Generate random integer | `random.randint(0, 100)` |
| Input Validation | Validate numeric input | `user_input.isdigit()` |
| String Replacement | String replacement operation | `input_str.replace('.', '')` |
| Variable Arguments | Accept variable number of arguments | `def my_sum(*numbers):` |
| Sum Initialization | Sum with initial value | `sum([1,2,3], start=0)` |
| Error Handling | Exception handling mechanism | `try: ... except Exception:` |
| Float Conversion | Float conversion and calculation | `float(run_time)` |
| Walrus Operator | Walrus operator (:=) | `while (run_time := input(...)):` |
| String Reversal | Reverse string order | `reversed(str)` |
| Index-Value Pairs | Get index-value pairs | `enumerate(reversed(...))` |
| ASCII Conversion | Character ASCII value conversion | `ord(char.upper())` |
| Digital Check and Conversion | Check if digit and Convert uppercase | `digit.isdigit()` and `upper()` |
| Built-in Conversion | Built-in base conversion function | `int('1A', 16)` |

## String Handling Skills

| Skill | Description | Example |
|-------|-------------|---------|
| String Slicing | Extract substring with indexes | `word[1:]` |
| String Formatting | Format strings with f-strings | `f'{word}way'` |
| String Splitting | Split string into list | `sentence.split()` |
| String Joining | Join list into string | `' '.join(word_list)` |
| Character Rotation | ROT13 encryption implementation | `chr(ord(c) + 13)` or `codecs.encode(word, 'rot13')` |
| Case Conversion | Convert to lowercase | `word.lower()` |
| String Sorting | Sort characters in string | `sorted('python')` |
| Case-insensitive Sort | Sort with key function | `sorted(s, key=str.lower)` |

## Video References

Each exercise includes a video tutorial for additional learning:
- Exercise 01: https://youtu.be/KDMuGX9QtNI
- Exercise 02: https://youtu.be/EDeZwyWfunM
- Exercise 03: https://youtu.be/Vajtow2DG3g
- Exercise 05: https://youtu.be/v4FxKzrBmNY
- Exercise 06: https://youtu.be/BwN0MegOAsY
- Exercise 08: https://youtu.be/wBn9m8wad0Y

## Note
The exercises focus on practical Python programming skills and include interactive elements for hands-on learning. Each exercise builds upon fundamental concepts while introducing new Python features and best practices.


