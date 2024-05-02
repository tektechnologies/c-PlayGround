# Functions

## Function Declaration and Definition in C++

In C++, a function declaration and definition are two separate parts of creating a function. 

1. **Function Declaration**: This is also known as a function prototype. It tells the compiler about the function name, return type, and parameters it accepts. A function declaration ends with a semicolon. It allows you to use the function before its actual definition in the code. 

    ```cpp
    // Function declaration
    int add(int a, int b); // This tells the compiler that there is a function named add which takes two integers as parameters and returns an integer.
    ```

2. **Function Definition**: This is where you provide the actual implementation of the function. It includes the function name, return type, parameters, and the code block that defines what the function does.

    ```cpp
    // Function definition
    int add(int a, int b) { // This defines the function add, which takes two integers as parameters and returns their sum.
        return a + b;
    }
    ```

Here, `add` is a function that takes two integers `a` and `b` as parameters and returns their sum, which is an integer.

In summary, the declaration tells the compiler about the function's existence, while the definition provides the actual implementation of the function.

- Parameters and arguments
- Return values
- Function overloading
