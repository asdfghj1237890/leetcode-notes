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
| Digital Check | Check if digit | `digit.isdigit()` |
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

## List & Tuple Skills

| Skill | Description | Example |
|-------|-------------|---------|
| Sequence Slicing | Get first/last elements | `seq[:1] + seq[-1:]` |
| List Memory Allocation | Dynamic memory management | `list.append(item)` will add memory space when the existing space is not enough |
| Tuple Efficiency | Fixed-size memory allocation | `tuple_data = (1,2,3)` is fixed size when it is created |
| Container Checking | Check if container is empty | `if not items:` |
| Dictionary Merging | Combine dictionaries | `{**d1, **d2}` |
| Type Checking | Verify data type | `isinstance(item, dict)` |
| Advanced Sorting | Multi-key sorting | `sorted(data, key=lambda x: (x[1], x[0]))` |
| Itemgetter Usage | Extract specific elements | `operator.itemgetter(1, 0)` |
| Formatted Output | Control string width/precision | `f'{last:12s}{first:10s}{grade:.1f}'` |
| Set Operations | Get unique elements | `set('independence')` |
| Element Counting | Count occurrences | `word.count(letter)` |
| Counter Usage | Efficient frequency counting | `Counter('independence').most_common(1)` |

## Video References

Each exercise includes a video tutorial for additional learning:
- Exercise 01: https://youtu.be/KDMuGX9QtNI
- Exercise 02: https://youtu.be/EDeZwyWfunM
- Exercise 03: https://youtu.be/Vajtow2DG3g
- Exercise 05: https://youtu.be/v4FxKzrBmNY
- Exercise 06: https://youtu.be/BwN0MegOAsY
- Exercise 08: https://youtu.be/wBn9m8wad0Y
- Exercise 09: https://youtu.be/teBer27fyek
- Exercise 10: https://youtu.be/dGSrJzQHiqc
- Exercise 11: https://youtu.be/nFq5kbxLkYY
- Exercise 12: https://youtu.be/powU_XZuylU
- Exercise 13: https://youtu.be/J48Am5fa27w

## Note
The exercises focus on practical Python programming skills and include interactive elements for hands-on learning. Each exercise builds upon fundamental concepts while introducing new Python features and best practices.


