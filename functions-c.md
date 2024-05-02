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

### Parameters and Arguments in C++

In C++, "parameters" and "arguments" are terminologies often used interchangeably, but they refer to different concepts within the context of functions.

1. **Parameters**: Parameters are the variables declared in a function's definition. They act as placeholders for the values that will be passed into the function when it is called. Parameters are part of the function's signature and are defined within the parentheses following the function name.

    ```cpp
    // Function definition with parameters
    int add(int a, int b) {
        return a + b;
    }
    ```

    In this example, `a` and `b` are parameters of the `add` function.

2. **Arguments**: Arguments, on the other hand, are the actual values passed to a function when it is called. They correspond to the parameters defined in the function declaration or definition. Arguments are specified within the parentheses following the function name during the function call.

    ```cpp
    // Function call with arguments
    int result = add(5, 3);
    ```

    Here, `5` and `3` are the arguments passed to the `add` function.

In summary, parameters are variables declared in the function definition, while arguments are the actual values passed to the function during its invocation. The arguments provided must match the parameters in number, order, and type.

- Return values
- Function overloading
