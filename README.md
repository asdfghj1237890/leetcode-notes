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

## Dict & Set Skills

| Skill | Description | Example |
|-------|-------------|---------|
| Safe Key Access | Get values without KeyError | `my_dict.get(key, default_none_value)` |
| Default Dictionaries | Automatic key initialization | `from collections import defaultdict` |
| Dictionary Views | Iterate key-value pairs | `for k, v in my_dict.items():` |
| Set Uniqueness | Remove duplicate elements | `unique = set([1,2,2,3])` |
| Key Collection | Get all dictionary keys | `my_dict.keys()` |
| Set Operations | Mathematical set operations (\|&^-) | `dict1.keys() \| dict2.keys()` (union) |

## File Handling Skills

| Skill | Description | Example |
|-------|-------------|---------|
| File Opening | Open files with different modes | `open(filename, 'r')` |
| Context Management | Automatic file closing | `with open(...) as f:` |
| CSV Processing | Read/write CSV files | `csv.reader(f, delimiter=':')` |
| JSON Handling | Parse and load JSON data | `json.load(json_file)` |
| Batch Processing | Process multiple files | `os.listdir(dirname)` |
| Path Manipulation | Combine file paths safely | `os.path.join(dirname, filename)` |
| File Format Detection | Check file extensions | `filename.endswith('.json')` |
| Memory Optimization | Read files line by line | `f.readline()` with walrus operator |
| Pretty Printing | Format complex structures | `pprint.pprint(data, sort_dicts=False)` |
| Delimiter Handling | Work with different separators | `csv_writer = csv.writer(f, delimiter='\t')` |
| Newline Control | Manage line endings | `newline=''` in open() |
| Data Serialization | Convert objects to JSON | `json.dump(data, file)` |
| File Type Filtering | Select specific file types | `glob.glob('*.json')` |

## Function Skills

| Skill | Description | Example |
|-------|-------------|---------|
| Default Parameters | Set default parameter values | `def func(name='World')` |
| Variable Scope | LEGB rule (Local, Enclosed, Global, Built-in) | `global`, `nonlocal` keywords |
| Keyword Arguments | Accept arbitrary keyword arguments | `def func(**kwargs)` |
| Function Dictionary | Store functions in dictionary | `ops = {'+': operator.add}` |
| Operator Module | Use built-in operator functions | `import operator` |
| Closure Functions | Remember enclosing scope | `def outer(): return inner` |
| Function Factories | Generate functions dynamically | `def factory(): return lambda` |

## Video References

Each exercise includes a video tutorial for additional learning:
- Playlist: https://youtube.com/playlist?list=PLA5TE2ITfeXSNSoqvV8u4QZjOqfK1L-_W
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
- Exercise 14: https://youtu.be/wd8YQTFHLzM
- Exercise 15: https://youtu.be/plARvm3RQXM
- Exercise 16: https://youtu.be/iV_K14vT_ZQ
- Exercise 17: https://youtu.be/eQnHwmXlPq4
- Exercise 18: https://youtu.be/GC5yQg2odqI
- Exercise 19: https://youtu.be/zktvhCOJPX0
- Exercise 20: https://youtu.be/YCrV2_wO4Cc
- Exercise 22: https://youtu.be/bSA1llDhX1I
- Exercise 23: https://youtu.be/0jHBF9-V9G0
- Exercise 25: https://youtu.be/cwm-UgM6oC4
- Exercise 26: https://youtu.be/btf2V4oyYaE
- Exercise 27: https://youtu.be/S6wIHzRhj8s

## Note
The exercises focus on practical Python programming skills and include interactive elements for hands-on learning. Each exercise builds upon fundamental concepts while introducing new Python features and best practices.


