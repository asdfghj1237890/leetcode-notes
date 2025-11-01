# LeetCode Notes

This repository contains Jupyter notebooks with coding exercises and their solutions, inspired by and adapted from Reuven M. Lerner's "Python Workout: 50 ten-minute exercises". Below is a summary of the exercises and key skills demonstrated.

## Python Tutor
http://pgbovine.net

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
| Character Rotation | ROT13 encryption implementation | `chr((ord(c.upper()) - 65 + 13) % 26 + 65)` or `codecs.encode(word, 'rot13')` |
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
| Operator Module | Use built-in operator functions | `import operator; operator.add(2,3)` |
| Lambda Functions | Anonymous functions for short operations | `lambda a, b: a + b` |
| Closure Functions | Remember enclosing scope | `def outer(): def inner(): ...; return inner` |
| Function Factories | Generate functions dynamically | `def factory(): return lambda x: x*2` |
| Returning Functions | Return a function from another function | `return password_gen` |
| Arbitrary Arguments | Accept variable number of arguments | `def my_sum(*numbers):` |
| Dynamic Attribute Handling | Accept and use arbitrary keyword arguments | `def myxml(tag, content='', **kwargs): ...` |

## Module & Package Skills

| Skill | Description | Example |
|-------|-------------|---------|
| Type Validation | Validate numeric input types | `if not isinstance(amount, (int, float)): raise ValueError('amount')` |
| Decimal Arithmetic | Precise monetary calculations | `from decimal import Decimal; Decimal('0.2')` |
| Package Structure | Create package with `__init__.py` and modules | `import tax.income_tax` |
| Import Path | Temporarily extend module search path | `import sys; sys.path.append('./data')` |

## Object & Class Skills

| Skill | Description | Example |
|-------|-------------|---------|
| Class & self | Initialize instance attributes | `def __init__(self, flavor): self.flavor = flavor` |
| Instance vs Class | Access class attribute from instances | `class Bowl: max_scoops = 3` |
| __str__/__repr__ | Custom printable/representation of objects | `def __repr__(self): return f'Bowl(scoops={self.scoops})'` |
| Inheritance & Override | Subclass and override attributes/methods | `class ExtraBowl(Bowl): max_scoops = 5` |
| super() initializer | Call parent constructor to avoid duplication | `super().__init__(color, 4)` |
| Class name lookup | Get class name of instance | `self.__class__.__name__` |
| f-string !r | Use repr formatting for clarity | `f"{self.color!r}"` |
| Subclass built-ins | Extend dict behavior safely | `class StrDict(dict): ...` |
| Dunder method override | Intercept item set/get | `def __setitem__(self, k, v): ...` |
| Nested comprehensions | Query across nested containers | `[a for ex in zoo.exhibits for a in ex.animals]` |
| Aggregation | Compute totals across objects | `sum(a.leg_num for ex in zoo.exhibits for a in ex.animals)` |

## Iterator & Generator Skills

| Skill | Description | Example |
|-------|-------------|---------|
| Iterator Protocol | Implement `__iter__` and `__next__`; raise `StopIteration` to end | `class MyEnumerate: def __iter__(self): return self; def __next__(self): ...` |
| Separate Iterator Class | Return a fresh iterator each time to avoid shared state | `class CycleList: def __iter__(self): return CycleIterator(data, n)` |
| Cycling with Modulo | Loop over data repeatedly using modular index | `value = data[i % len(data)]` |
| Generator Function | Use `yield` to lazily produce values | `def word_generator(f, n): ... yield word` |
| Early Termination | Stop a generator with `return` when a limit is reached | `if count >= n: return` |
| Generator Expression | Inline lazy sequence construction | `(int(d) for d in str(num) if d.isnumeric())` |
| Stateful Infinite Generator | Preserve state between yields for ongoing values | `def elapsed_time_gen(): yield now - last` |

## Comprehension & Generator Skills

| Skill | Description | Example |
|-------|-------------|---------|
| List Comprehension | Generate lists with expressions | `[abs(x) for x in numbers]` |
| Nested List Comprehension | Flatten 2D lists | `[sub for row in data for sub in row]` |
| Dict Comprehension | Generate dicts from iterables | `{k: v for k, v in pairs}` |
| Set Comprehension | Generate sets from iterables | `{x for x in data}` |
| Conditional Comprehension | Add if condition in comprehension | `[x for x in data if x > 0]` |
| Filter Function | Filter elements with a function | `filter(str.isdigit, data)` |
| Map Function | Apply function to all elements | `map(abs, numbers)` |
| Generator Expression | Lazy evaluation of sequences | `(x*x for x in range(10))` |
| File Processing with Comprehension | Process file lines/words | `' '.join([pl_word(w) for l in f for w in l.split()])` |
| Dict/Set Flip | Flip dict keys and values | `{v: k for k, v in d.items()}` |

## Appendix A - Additional Skills

| Skill | Description | Example |
|-------|-------------|---------|
| Combinations (itertools) | List all 2-combinations; useful for pair checks | `from itertools import combinations; list(combinations(data, 2))` |
| Counter.most_common | Get most frequent element efficiently | `Counter(data).most_common(1)[0]` returns `(element, count)` tuple |
| Set subtraction | Find missing numbers from 1..n via set difference | `set(range(1, len(data)+2)) - set(data)` for missing in [1..n+1] |
| Stack via list/subclass | Use list methods or subclass list for stack ops | `stack = []; stack.append(x); stack.pop()` |
| Bracket validation (stack) | Validate parentheses/brackets using push/pop | `stack and b == stack.pop()` |
| Move zeroes to end | Shift all zeroes to the list's end | `for _ in range(data.count(0)): data.remove(0); data.append(0)` |
| Common prefix (zip) | Use zip to align chars; stop at first mismatch | `"".join(c[0] for c in zip(*strs) if len(set(c)) == 1)` |
| Reverse integer digits | Reverse digits with slicing and preserve sign | `int(str(abs(x))[::-1]) * (1 if x >= 0 else -1)` |
| Reverse 8-bit binary | Format to 8 bits, reverse, parse base 2 | `int(f'{n:08b}'[::-1], 2)` |
| Roman numerals to int | Sum symbols plus subtractive pairs | `sum(roman[c] for c in s) + sum(v for k, v in special.items() if k in s)` |

## Video References

Each exercise includes a video tutorial for additional learning:
- Playlist: https://youtube.com/playlist?list=PLA5TE2ITfeXSNSoqvV8u4QZjOqfK1L-_W
- Exercise 01: Warm-up----Number Guessing Game — https://youtu.be/KDMuGX9QtNI
- Exercise 02: Sum a Series of Numbers — https://youtu.be/EDeZwyWfunM
- Exercise 03: Calculate Average Running Time — https://youtu.be/Vajtow2DG3g
- Exercise 04: Convert Hexadecimal to Decimal — (no video)
- Exercise 05: Pig Latin — https://youtu.be/v4FxKzrBmNY
- Exercise 06: Pig Latin - Sentence Translator — https://youtu.be/BwN0MegOAsY
- Exercise 07: ROT13 Encryption — (no video)
- Exercise 08: Character Sorting — https://youtu.be/wBn9m8wad0YL
- Exercise 09: Extract and Combine First and Last Elements from Different Containers — https://youtu.be/teBer27fyek
- Exercise 10: Universal Sum Function — https://youtu.be/dGSrJzQHiqc
- Exercise 11: Sort Contact Information by Name — https://youtu.be/nFq5kbxLkYY
- Exercise 12: Output Container Data with Formatting — https://youtu.be/powU_XZuylU
- Exercise 13: Find Most Repeated Letter in a Word — https://youtu.be/J48Am5fa27w
- Exercise 14: Restaurant Ordering System — https://youtu.be/wd8YQTFHLzM
- Exercise 15: Rainfall Database — https://youtu.be/plARvm3RQXM
- Exercise 16: Dictionary Key/Value Sorter — https://youtu.be/iV_K14vT_ZQ
- Exercise 17: Compare Two Dictionaries — https://youtu.be/eQnHwmXlPq4
- Exercise 18: Read the Last Line of a File — https://youtu.be/GC5yQg2odqI
- Exercise 19: Extract Login Account Information — https://youtu.be/zktvhCOJPX0
- Exercise 20: Count Characters, Words and Lines in a File — https://youtu.be/YCrV2_wO4Cc
- Exercise 21: Find the Longest Word in a File — (no video)
- Exercise 22: Reading and Writing CSV Files — https://youtu.be/bSA1llDhX1I
- Exercise 23: Reading JSON Files — https://youtu.be/0jHBF9-V9G0
- Exercise 25: XML Generator — https://youtu.be/cwm-UgM6oC4
- Exercise 26: Simple Prefix Calculator — https://youtu.be/btf2V4oyYaE
- Exercise 27: Custom Password Generator — https://youtu.be/S6wIHzRhj8s
- Exercise 29: Sum Only Numbers in Data — https://youtu.be/GXK_RHEdv_s
- Exercise 30: Flatten 2D List Using Nested List Comprehension — https://youtu.be/gYG9qZyIu0g
- Exercise 31: Pig Latin - File Translator — https://youtu.be/0ui1zWaDSSU
- Exercise 32: Flip a dict's keys and values — https://youtu.be/DDAYafF7KmQ
- Exercise 35: Hebrew Number Cipher (Part I) — https://youtu.be/aBqi0HhBdiA
- Exercise 35: Hebrew Number Cipher (Part II) — https://youtu.be/852LFBEK0BI
- Exercise 36: Income Tax Calculation Module — https://youtu.be/dGwEEiXqIQY
- Exercise 37: Function Menu Module — https://youtu.be/Xe-HKd32DtY
- Exercise 38: Ice Cream Scoop — https://youtu.be/uAItLgO0hCc
- Exercise 39: Ice Cream Bowl — https://youtu.be/PevJYLbs4vk
- Exercise 40: Class Attribute - Ice Cream Bowl Limit — https://youtu.be/HTUbvK7Vlbs
- Exercise 41: Extra Large Ice Cream Bowl — https://youtu.be/q7XO4knadH4
- Exercise 42: Custom dict with String Keys — https://youtu.be/OSkaqQ5Ukg4
- Exercise 43: Animal Class — https://youtu.be/or0UPz7QL8U
- Exercise 44: Animal Exhibition Area Class — https://youtu.be/6dBzsZUZOy8
- Exercise 45: Zoo Class — https://youtu.be/44vHQ5l4u3s
- Exercise 46: Custom Iterable Container — https://youtu.be/8p5CMpWh1KM
- Exercise 47: Cycle Iterator — https://youtu.be/4GLb_bYC9wA
- Exercise 48: File Word Generator — (no video)
- Exercise 49: Generator Expressions — (no video)
- Exercise 50: Elapsed Time Generator — https://youtu.be/qof3fxYBn8U

## Note
The exercises focus on practical Python programming skills and include interactive elements for hands-on learning. Each exercise builds upon fundamental concepts while introducing new Python features and best practices.


