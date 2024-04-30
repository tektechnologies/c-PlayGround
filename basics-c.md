# Basics of C++

- Hello World program - code from Hacker Rank

```cpp
#include <iostream>
#include <cstdio>
using namespace std;

int main() {
    printf("Hello, World!");
    return 0;
}
```

- Comments

```cpp

// This is a single-line comment in C++

/*
This is a multi-line comment
in C++. It can span multiple lines
*/

```

- Data types and variables

In C++, there are several data types that can be used to define variables. Here are some of the commonly used data types:

1. **Integer Types:**
   - `int`: Typically a 32-bit signed integer.
   - `short`: Typically a 16-bit signed integer.
   - `long`: Typically a 32-bit or 64-bit signed integer.
   - `long long`: At least 64 bits, introduced in C++11.

2. **Floating-Point Types:**
   - `float`: Single-precision floating-point type.
   - `double`: Double-precision floating-point type.
   - `long double`: Extended-precision floating-point type.

3. **Character Types:**
   - `char`: Typically a single-byte (8-bit) character.
   - `wchar_t`: Wide character type, used for Unicode characters.
   - `char16_t`: 16-bit Unicode character type introduced in C++11.
   - `char32_t`: 32-bit Unicode character type introduced in C++11.

4. **Boolean Type:**
   - `bool`: Represents boolean values `true` or `false`.

5. **Void Type:**
   - `void`: Represents the absence of type.

6. **User-Defined Types:**
   - C++ allows defining custom data types using `struct`, `class`, `enum`, and `union`.

Additionally, C++ also supports modifiers like `signed`, `unsigned`, and `const` that can be used with these data types to modify their behavior or constraints.

For example:

- `signed int` and `int` are typically the same, but `signed int` explicitly denotes the signedness.
- `unsigned int` represents only non-negative integers.

These are the fundamental data types in C++ that are used to declare variables and functions, and they form the building blocks for more complex data structures and types.

## variables

In C++, variables are used to store data that can be manipulated and accessed within a program. Each variable has a specific data type, which determines the kind of data it can store (such as integers, floating-point numbers, characters, etc.). Variables in C++ have the following characteristics:

1. **Name:** Variables have names that are used to refer to them in the program. Variable names must adhere to certain rules, such as starting with a letter or underscore, and can contain letters, digits, and underscores.

2. **Data Type:** Every variable in C++ has a data type that defines the kind of data it can hold, such as `int`, `float`, `char`, etc.

3. **Value:** Variables can hold a value of the specified data type. The value can be assigned initially during declaration or later in the program.

4. **Memory Location:** Each variable is stored in a specific memory location in the computer's memory, allowing the program to access and modify its value.

5. **Scope:** Variables have a scope that determines where they can be accessed within the program. Variables declared inside a block of code are typically local to that block, while variables declared outside all blocks have global scope.

Here's an example of variable declaration and assignment in C++:

```cpp
#include <iostream>

int main() {
    // Declaration and initialization of variables
    int age = 25;
    float height = 5.9;
    char grade = 'A';

    // Output the values of variables
    std::cout << "Age: " << age << std::endl;
    std::cout << "Height: " << height << " feet" << std::endl;
    std::cout << "Grade: " << grade << std::endl;

    return 0;
}

In this example:

- `age`, `height`, and `grade` are variables.
- They are declared with specific data types (`int`, `float`, and `char` respectively).
- They are initialized with values (`25`, `5.9`, and `'A'` respectively).
- Their values are outputted using `std::cout`.
 
```

- Constants

In C++, constants are identifiers whose values cannot be changed during the execution of the program. They provide a way to define fixed values that remain constant throughout the program's execution. Constants in C++ have the following characteristics:

1. **Value:** Constants have a fixed value that cannot be modified once they are defined.

2. **Data Type:** Like variables, constants also have a data type which determines the type of value they hold (e.g., integer, floating-point, character, etc.).

3. **Name:** Constants are given a name, just like variables, which is used to refer to them in the program.

4. **Scope:** Constants can have either local or global scope, depending on where they are declared.

5. **Initialization:** Constants must be initialized at the time of declaration.

In C++, there are two ways to define constants:

1. **Using `const` keyword:** Constants can be defined using the `const` keyword followed by the data type and the constant name. For example:

```cpp
   const int MAX_VALUE = 100;

```

- Using #define preprocessor directive: Constants can also be defined using the #define preprocessor directive. For example:

### define PI 3.14159

```cpp

#include <iostream>

int main() {
    const int MAX_VALUE = 100;
    const double PI = 3.14159;

    std::cout << "Max Value: " << MAX_VALUE << std::endl;
    std::cout << "Value of PI: " << PI << std::endl;

    return 0;
}

```

In this example:

- MAX_VALUE and PI are constants.
- They are defined with specific data types (int and double respectively).
- Their values cannot be changed during the program's execution.
- Their values are outputted using std::cout.

## Operators

In C++, operators are symbols that perform operations on operands. They are used to manipulate data and perform calculations. C++ supports a wide range of operators, which can be categorized into several groups:

1. **Arithmetic Operators:**
   - Addition `+`
   - Subtraction `-`
   - Multiplication `*`
   - Division `/`
   - Modulus `%` (remainder of division)

2. **Assignment Operators:**
   - Assignment `=`
   - Addition assignment `+=`
   - Subtraction assignment `-=`
   - Multiplication assignment `*=`
   - Division assignment `/=`
   - Modulus assignment `%=` 
   - Bitwise AND assignment `&=`
   - Bitwise OR assignment `|=`
   - Bitwise XOR assignment `^=`
   - Bitwise left shift assignment `<<=`
   - Bitwise right shift assignment `>>=`

3. **Comparison Operators:**
   - Equal to `==`
   - Not equal to `!=`
   - Greater than `>`
   - Less than `<`
   - Greater than or equal to `>=`
   - Less than or equal to `<=`

4. **Logical Operators:**
   - Logical AND `&&`
   - Logical OR `||`
   - Logical NOT `!`

5. **Bitwise Operators:**
   - Bitwise AND `&`
   - Bitwise OR `|`
   - Bitwise XOR `^`
   - Bitwise NOT `~`
   - Left shift `<<`
   - Right shift `>>`

6. **Increment and Decrement Operators:**
   - Increment `++`
   - Decrement `--`

7. **Conditional Operator (Ternary Operator):**
   - Conditional expression `? :`

8. **Member Access Operators:**
   - Dot `.` (for accessing members of objects or structures)
   - Arrow `->` (for accessing members through pointers)

9. **Sizeof Operator:**
   - Sizeof `sizeof`

10. **Comma Operator:**
    - Comma `,` (evaluates its operands from left to right and returns the value of the rightmost operand)

These are the primary operators in C++. Each operator serves a specific purpose and is used in different contexts to perform various operations on data.
