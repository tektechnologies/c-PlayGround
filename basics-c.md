# Basics of C++

- Hello World program - code from Hacker Rank

```c++
#include <iostream>
#include <cstdio>
using namespace std;

int main() {
    printf("Hello, World!");
    return 0;
}
```

- Comments

```c++

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

- Constants

- Operators
