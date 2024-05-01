# Control Structures

- Decision making (if-else, switch)

## Decision Making in C++

In C++, decision-making can be implemented using if-else statements and switch statements. These constructs allow you to control the flow of your program based on certain conditions. Here's how you can use them:

### If-Else Statements

The `if-else` statement evaluates a condition and executes a block of code if the condition is true, otherwise, it executes another block of code.

```cpp
if (condition) {
    // Code block to execute if condition is true
} else {
    // Code block to execute if condition is false
}

int x = 10;
if (x > 5) {
    cout << "x is greater than 5";
} else {
    cout << "x is less than or equal to 5";
}

switch (expression) {
    case constant1:
        // Code block to execute if expression equals constant1
        break;
    case constant2:
        // Code block to execute if expression equals constant2
        break;
    // Add more cases as needed
    default:
        // Code block to execute if expression doesn't match any case
}

int day = 3;
switch (day) {
    case 1:
        cout << "Monday";
        break;
    case 2:
        cout << "Tuesday";
        break;
    // Continue with other cases as needed
    default:
        cout << "Invalid day";
}

```


- Loops (for, while, do-while)


- Break and continue statements
