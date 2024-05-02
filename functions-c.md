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

### Return Values in C++

In C++, a return value is the value that a function sends back to the code that called it. It allows functions to compute a result and pass it back to the caller for further use.

When a function is declared to return a value, its declaration includes the data type of the value that it returns. This is specified before the function name in the declaration or definition.

Here's how you declare a function that returns a value:

```cpp
// Function declaration with return type
int multiply(int a, int b); // Declares a function named multiply that returns an integer value


// Function definition with return type
int multiply(int a, int b) {
    return a * b; // Returns the product of a and b
}

// In this example, the multiply function takes two integers as parameters and returns their product. The return statement is used to send back the computed result to the caller.

// When calling a function that returns a value, you can capture that value using a variable or use it directly in an expression:

int result = multiply(5, 3); // Calling multiply function and capturing the returned value

```

- The value returned by the multiply function (in this case, the product of 5 and 3) is stored in the variable result.

- In summary, return values in C++ enable functions to compute results and send them back to the calling code for further processing or use.

### Function Overloading in C++

Function overloading in C++ allows you to define multiple functions with the same name but with different parameters. This enables you to use the same function name for different operations based on the types or number of arguments passed to it. Function overloading provides a way to create more readable and expressive code by using intuitive function names for similar operations.

Here's an example to illustrate function overloading:

```cpp
#include <iostream>

// Function to add two integers
int add(int a, int b) {
    return a + b;
}

// Overloaded function to add two doubles
double add(double a, double b) {
    return a + b;
}

int main() {
    // Calling the add function with integers
    std::cout << "Sum of integers: " << add(5, 3) << std::endl;

    // Calling the add function with doubles
    std::cout << "Sum of doubles: " << add(5.5, 3.3) << std::endl;

    return 0;
}

```

In this example, we have two add functions: one that takes two integers and another that takes two doubles as parameters. These functions have the same name (add) but different parameter types. Depending on the arguments passed during the function call, the compiler selects the appropriate version of the function to execute.

Function overloading is resolved at compile time, and the compiler determines which function to call based on the number and types of arguments provided.

Key points about function overloading:

Functions must have different parameter lists (number, types, or order of parameters) to be overloaded.
Return types do not play a role in overloading. Two functions can have the same parameter list but different return types and still be considered overloaded.
Overloaded functions can have different access specifiers (public, private, protected).
Overloading can be applied to member functions of classes as well as global functions.
Function overloading is a powerful feature of C++ that allows you to write concise and expressive code by providing multiple ways to accomplish similar tasks.
