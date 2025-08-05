# Arrays-and-strings

##  Aim
To study the concepts of arrays and strings in C++ and implement basic operations.

##  Objectives
- Understand the declaration, initialization, and traversal of arrays and strings in C++.
- Perform common array operations:
  - Searching
  - Sum and average
  - Finding maximum and minimum
- Explore different ways to declare and initialize strings.
- Implement string operations:
  - Concatenation
  - Reversal
  - Palindrome checking
- Enhance basic problem-solving skills using arrays and strings.

##  Theory

###  Arrays in C++
An array is a **linear data structure** that stores multiple elements of the same data type in contiguous memory locations.  
Each element is accessed using an **index (0-based)**.

####  Types of Arrays
- **One-Dimensional Array**  
  `int arr[5] = {1, 2, 3, 4, 5};`
- **Two-Dimensional Array**  
  `int matrix[2][3] = {{1, 2, 3}, {4, 5, 6}};`

####  Common Operations on Arrays
- **Traversal** – Access elements using loops  
- **Searching** – Linear or binary search  
- **Aggregation** – Sum, average, min, max  
- **Insertion/Deletion** – Done manually (in static arrays)

####  Advantages
- Easy and fast access with index  
- Simple declaration and use  

####  Limitations
- Fixed size  
- Costly insert/delete operations  

###  Strings in C++
Strings are sequences of characters used to store and manipulate text.

####  C-Style Strings
Defined as character arrays ending with `\0`  
Example: `char name[] = "Mishree";`

####  C++ Strings (STL `string`)
Introduced via `<string>` header  
More powerful and object-oriented  
Example: `string name = "Mishree";`

###  Common String Functions

| Function     | Syntax                  | Description                          | Example                        |
|--------------|-------------------------|--------------------------------------|--------------------------------|
| `length()`   | `str.length()`          | Length of string                     | `"Hello".length()` → 5        |
| `size()`     | `str.size()`            | Same as length                       | `"Hi".size()` → 2             |
| `append()`   | `str1.append(str2)`     | Concatenate str2 to str1             | `"Hi".append("There")` → "HiThere" |
| `+` operator | `str1 + str2`           | Concatenate strings                  | `"Hi" + "There"` → "HiThere"  |
| `at(index)`  | `str.at(2)`             | Character at index with bounds check | `"Hello".at(1)` → 'e'         |
| `[]`         | `str[i]`                | Access char at index (no bounds check) | `"Hello"[1]` → 'e'           |
| `substr()`   | `str.substr(start, len)`| Substring from start                 | `"Hello".substr(1,3)` → "ell" |
| `find()`     | `str.find("sub")`       | Index of char/substr                 | `"hello".find("e")` → 1       |
| `compare()`  | `str1.compare(str2)`    | Returns 0 if equal                   | `"abc".compare("abc")` → 0    |
| `empty()`    | `str.empty()`           | Checks if string is empty            | `"" → true`                   |
| `clear()`    | `str.clear()`           | Clears string content                | `"test".clear()` → ""         |
| `c_str()`    | `str.c_str()`           | Converts to C-style string           | Used with legacy C functions  |
| `reverse()`  | `reverse(str.begin(), str.end())` | Reverses string               | `"abc"` → `"cba"`             |

###  String Operations
- **Concatenation**: Using `+` or `.append()`
- **Reversal**: Using loop or `reverse()` function
- **Palindrome Check**: Compare original and reversed string

###  Arrays vs Strings Comparison

| Feature               | C-style String (`char[]`) | C++ `string` Class     |
|-----------------------|---------------------------|-------------------------|
| Header File           | `<cstring>`               | `<string>`              |
| Null-Terminated       | Yes                       | No                      |
| Declaration           | `char str[10] = "Hi";`    | `string str = "Hi";`    |
| Length Calculation    | `strlen(str)`             | `str.length()`          |
| Concatenation         | `strcat()`                | `+`, `append()`         |
| Comparison            | `strcmp()`                | `==`, `compare()`       |
| Safer to Use          | ❌                        | ✅                      |
| Memory Management     | Manual                    | Automatic               |
| Object-Oriented       | ❌                        | ✅                      |

## 🔧 Program Descriptions

### 1. Print Array Elements
- Input array from user
- Use loop to display elements

### 2. Search Number in Array
- Use a loop and flag to check if a number exists

### 3. Sum & Average of Array
- Calculate total using loop
- Average = total / count

### 4. Find Maximum and Minimum
- Traverse and use conditions to track max/min

### 5. String Declaration Methods
- Using: `char str[] = "Hello";`
- Using: `string str = "World";`

### 6. String Concatenation
- With `+` operator or `.append()`

### 7. Print String in Reverse
- Use a loop or `reverse()` function

### 8. Palindrome Check
- Compare characters from both ends  
- Or reverse and compare with original

##  Concepts Used
- Array Traversal & Manipulation
- String Handling (C-style & C++ style)
- Loops (`for`, `while`)
- Conditional Statements (`if-else`)
- String Functions from `<string>` and `<algorithm>`

##  Conclusion
This experiment helped us explore one of the most fundamental concepts in C++: arrays and strings. By implementing common operations like traversal, search, sum, and string manipulation, we strengthened our understanding of data storage and manipulation. We also compared C-style and modern C++ strings, and understood the importance of string handling in real-world applications. These skills form the basis for more advanced topics in programming and data structures.
