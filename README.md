# What is a Computer Program?

A **computer program** is a collection of instructions that can be executed by a computer to perform a specific task.

# What is Computer Programming?

**Computer programming** is the process of designing and building an executable computer program to accomplish a specific computing result or to perform a specific task.

## Program and Programming

A **computer program** is usually written by a computer programmer in a programming language. From the program in its human-readable form of source code, a compiler can derive machine code—a form consisting of instructions that the computer can directly execute. Alternatively, a computer program may be executed with the aid of an interpreter.

- **Source Code/High-Level Language**: Understandable by human beings  
- **Machine Code (Binary code)** (0 and 1) / **Low-Level Language**: Understandable by computer

### Compiler

The name "compiler" is primarily used for programs that translate source code from a high-level programming language to a lower-level language (e.g., machine code) to create an executable program.

### Interpreter

An **interpreter** is a program that executes instructions written in a high-level language.

### Compiler vs Interpreter

An interpreter translates just one statement of the program at a time into machine code. A compiler scans the entire program and translates the whole of it into machine code at once.

---

## Programming Cycle in C++

1. Think about what the program is supposed to do.
2. Edit Program (comment program and then write code)
3. Save Program
4. Compile Program
5. Fix Syntax Errors (Go back to Think above)
6. Run/Test Program
7. Fix Logic Errors (Go back to Think above)
8. Run Program

---

## Algorithm

- A sequence of instructions.
- A procedure or formula for solving a problem.
- Often used for calculation, data processing, and programming.
- Algorithms can be expressed in any language.

### Example of Algorithm in Programming

Algorithm to add two numbers entered by the user:

1. **Start**
2. **Declare variables** `num1`, `num2`, and `sum`.
3. **Read values** `num1` and `num2`.
4. **Add** `num1` and `num2` and assign the result to `sum`. `sum <- num1 + num2`
5. **Display** `sum`
6. **Stop**

---

## Pseudocode

- Pseudo code (which means fake code, because it’s not really programming code) specifies the steps required to accomplish the task.
- **Pseudocode** is a type of structured English that is used to specify an algorithm.
- Pseudocode cannot be compiled or executed, and there are no real formatting or syntax rules.

---

## Programming

Programming is the process of taking an **algorithm** and encoding it into a notation, a **programming language**, so that it can be executed by a computer. Programming is often the way that we create a representation for our solutions. Algorithms describe the solution to a problem in terms of the data needed to represent the problem instance and the set of steps necessary to produce the intended result. **Programming languages** must provide a notational way to represent both the process and the data.

---

## Difference between Algorithm, Pseudocode, and Program

- **Algorithm**: Systematic logical approach that is a well-defined, step-by-step procedure that allows a computer to solve a problem.
- **Pseudocode**: A simpler version of programming code in plain English, using short phrases to write code for a program before it is implemented in a specific programming language.
- **Program**: The exact code written for a problem, following all the rules of the programming language.

---

## Source Code

**Source code** is the language or string of words, numbers, letters, and symbols that a computer programmer uses. In computing, source code is any collection of code, with or without comments, written using a human-readable programming language, usually as plain text. The source code of a program is specially designed to facilitate the work of computer programmers, who specify the actions to be performed by a computer mostly by writing source code. The source code is often transformed by an assembler or compiler into binary machine code that can be executed by the computer.

---

## Example of C Language Source Code

```c
#include <stdio.h>

int main() {
    // printf displays the string inside quotation
    printf("Hello, World!");
    return 0;
}
```

## Example of C++ Language Source Code

```cpp
#include <iostream> // Include the iostream header: This header file is required for input (cin) and output (cout) operations.
using namespace std; // Using namespace std: Allows usage of symbols in the std namespace without prefixing with std::.

int main() {
    // cout displays the string inside quotation
    cout << "Hello, World!" << endl;
    return 0;
}
```
### Explanation:

- **`#include <iostream>`**: This header file is required for input (`cin`) and output (`cout`) operations.
- **`using namespace std;`**: Allows usage of symbols in the `std` namespace without prefixing with `std::`.
- **`int main()`**: The main function where execution begins.
- **`cout << "Hello, World!" << endl;`**: Prints "Hello, World!" to the console and moves the cursor to the next line.
- **`return 0;`**: Indicates that the program ended successfully.

# ARITHMETIC EXPRESSION & PRECEDENCE Operators in C++

An operator is a symbol that tells the compiler to perform specific mathematical or logical functions.

C++ language is rich in built-in operators and provides the following types of operators:

- Arithmetic Operators
- Relational Operators
- Logical Operators
- Bitwise Operators
- Assignment Operators
- Misc Operators

## Arithmetic Operators

The following table shows all the arithmetic operators supported by the C++ language. Assume variable `A` holds 10 and variable `B` holds 20 then:

| Operator | Description                                                | Example        |
|----------|------------------------------------------------------------|----------------|
| `+`      | Adds two operands                                          | `A + B = 30`   |
| `-`      | Subtracts second operand from the first.                   | `A - B = -10`  |
| `*`      | Multiplies both operands.                                  | `A * B = 200`  |
| `/`      | Divides numerator by denominator.                           | `A / B = 0.5`  |
| `%`      | Modulus Operator, gives remainder after integer division.  | `B % A = 0`    |
| `++`     | Increment operator increases the integer value by one.     | `A++`          |
| `--`     | Decrement operator decreases the integer value by one.     | `A--`          |

### Example: Arithmetic Operators

```cpp
// Working of arithmetic operators
#include <iostream>
using namespace std;

int main() {
    int a = 9, b = 4, c;
    c = a + b;
    cout << "a + b = " << c << endl;
    c = a - b;
    cout << "a - b = " << c << endl;
    c = a * b;
    cout << "a * b = " << c << endl;
    c = a / b;
    cout << "a / b = " << c << endl;
    c = a % b;
    cout << "Remainder when a divided by b = " << c << endl;
    return 0;
}
```
# Relational Operators in C++

The following table shows the relational operators supported by C++. Assume variable `A` holds 10 and variable `B` holds 20.

| Operator | Description                                               | Example                   |
|----------|-----------------------------------------------------------|---------------------------|
| `==`     | Checks if the values of two operands are equal.          | `(A == B)` is not true.   |
| `!=`     | Checks if the values of two operands are not equal.      | `(A != B)` is true.       |
| `>`      | Checks if the left operand is greater than the right.    | `(A > B)` is not true.    |
| `<`      | Checks if the left operand is less than the right.       | `(A < B)` is true.        |
| `>=`     | Checks if the left operand is greater than or equal.     | `(A >= B)` is not true.   |
| `<=`     | Checks if the left operand is less than or equal.        | `(A <= B)` is true.       |

## Example: Relational Operators

```cpp
#include <iostream>
using namespace std;

int main() {
    int a = 5, b = 5, c = 10;
    
    cout << a << " == " << b << " is " << (a == b) << endl;
    cout << a << " == " << c << " is " << (a == c) << endl;
    cout << a << " > " << b << " is " << (a > b) << endl;
    cout << a << " > " << c << " is " << (a > c) << endl;
    cout << a << " < " << b << " is " << (a < b) << endl;
    cout << a << " < " << c << " is " << (a < c) << endl;
    cout << a << " != " << b << " is " << (a != b) << endl;
    cout << a << " != " << c << " is " << (a != c) << endl;
    cout << a << " >= " << b << " is " << (a >= b) << endl;
    cout << a << " >= " << c << " is " << (a >= c) << endl;
    cout << a << " <= " << b << " is " << (a <= b) << endl;
    cout << a << " <= " << c << " is " << (a <= c) << endl;
    return 0;
}
```
# Logical Operators in C++

The following table shows the logical operators supported by C++. Assume variable `A` holds 1 and variable `B` holds 0.

| Operator | Description                                              | Example                     |
|----------|----------------------------------------------------------|-----------------------------|
| `&&`     | Logical AND operator; true if both operands are non-zero | `(A && B)` is false.        |
| `||`     | Logical OR operator; true if at least one operand is non-zero | `(A || B)` is true.     |
| `!`      | Logical NOT operator; reverses the logical state of its operand | `!(A && B)` is true. |

## Example: Logical Operators

```cpp
#include <iostream>
using namespace std;

int main() {
    int a = 5, b = 10;
    cout << ((a < b) && (b > a)) << endl; // true
    cout << ((a > b) || (b > a)) << endl; // true
    cout << !(a == b) << endl; // true
    return 0;
}
```
# Bitwise Operators in C++

Bitwise operators perform bit-by-bit operations. The truth tables for `&`, `|`, and `^` are as follows:

| p | q | p & q | p | q | p ^ q |
|---|---|-------|---|---|-------|
| 0 | 0 |   0   | 0 | 0 |   0   |
| 0 | 1 |   0   | 0 | 1 |   1   |
| 1 | 0 |   0   | 1 | 0 |   1   |
| 1 | 1 |   1   | 1 | 1 |   0   |

Assuming `A = 60` and `B = 13`, their binary representations are:

A = 0011 1100 B = 0000 1101


| Operator | Description                          | Example          |
|----------|--------------------------------------|------------------|
| `&`      | Binary AND operator                  | `A & B = 12`     |
| `|`      | Binary OR operator                   | `A | B = 61`     |
| `^`      | Binary XOR operator                  | `A ^ B = 49`     |
| `~`      | Binary One's Complement operator     | `~A = 192`       |

## Example: Bitwise Operators

```cpp
#include <iostream>
using namespace std;

int main() {
    unsigned char a = 5; // a = 00000101
    unsigned char b = 9; // b = 00001001

    cout << "a & b = " << (a & b) << endl; // Bitwise AND
    cout << "a | b = " << (a | b) << endl; // Bitwise OR
    cout << "a ^ b = " << (a ^ b) << endl; // Bitwise XOR
    cout << "~a = " << (int)(~a) << endl;   // Bitwise NOT

    return 0;
}
```
# Assignment Operators in C++

The following table lists the assignment operators supported by C++.

| Operator | Description                                          | Example           |
|----------|------------------------------------------------------|-------------------|
| `=`      | Simple assignment operator                            | `C = A + B`       |
| `+=`     | Add AND assignment operator; adds right operand to left | `C += A`        |
| `-=`     | Subtract AND assignment operator; subtracts right operand from left | `C -= A`    |
| `*=`     | Multiply AND assignment operator                      | `C *= A`          |
| `/=`     | Divide AND assignment operator                        | `C /= A`          |
| `%=`     | Modulus AND assignment operator                       | `C %= A`          |

## Example: Assignment Operators

```cpp
#include <iostream>
using namespace std;

int main() {
    int a = 10, c;
    c = a;
    cout << "c = " << c << endl; // c = 10
    c += a;
    cout << "c = " << c << endl; // c = 20
    c -= a;
    cout << "c = " << c << endl; // c = 10
    c *= a;
    cout << "c = " << c << endl; // c = 100
    c /= a;
    cout << "c = " << c << endl; // c = 10
    c %= a;
    cout << "c = " << c << endl; // c = 0
    return 0;
}
```
# Miscellaneous Operators in C++

## sizeof Operator

The `sizeof` operator returns the size of a variable in bytes.

### Example: sizeof Operator

```cpp
#include <iostream>
using namespace std;

int main() {
    int a;
    float b;
    double c;
    char d;
    cout << "Size of a = " << sizeof(a) << " bytes" << endl; // Size of a = 4 bytes
    cout << "Size of b = " << sizeof(b) << " bytes" << endl; // Size of b = 4 bytes
    cout << "Size of c = " << sizeof(c) << " bytes" << endl; // Size of c = 8 bytes
    cout << "Size of d = " << sizeof(d) << " bytes" << endl; // Size of d = 1 byte
    return 0;
}
```
# Conditional Operator

The conditional operator is a shorthand for the if-else statement. Its syntax is:

condition ? expression1 : expression2;


### Example: Conditional Operator

```cpp
#include <iostream>
using namespace std;

int main() {
    int a = 5, b = 10;
    cout << "Max: " << (a > b ? a : b) << endl; // Max: 10
    return 0;
}
```
