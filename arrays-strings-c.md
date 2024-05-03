# Arrays and Strings

## In C++, you can declare arrays using the following syntax

```cpp
// Syntax 1: Type arrayName[ arraySize ];
int integers[5]; // Declares an array of 5 integers

// Syntax 2: Type arrayName[] = { value1, value2, ..., valueN };
int primes[] = {2, 3, 5, 7, 11}; // Declares an array of integers with size inferred from the number of initializers

// Syntax 3: Type *arrayName = new Type[arraySize];
int *dynamicArray = new int[10]; // Declares a dynamically allocated array of 10 integers

// Syntax 4: Using std::array from the <array> header (requires C++11 or later)
#include <array>
std::array<int, 5> arr = {1, 2, 3, 4, 5}; // Declares an array of 5 integers using std::array

// Syntax 5: Using std::vector from the <vector> header (requires C++11 or later)
#include <vector>
std::vector<int> vec(10); // Declares a vector (dynamic array) of 10 integers

```

## Accessing array elements

```cpp
// Declare an array
int arr[5] = {10, 20, 30, 40, 50};

// Accessing elements of the array
int firstElement = arr[0];   // Accesses the first element (index 0)
int secondElement = arr[1];  // Accesses the second element (index 1)
int thirdElement = arr[2];   // Accesses the third element (index 2)
// and so on...

// You can also modify array elements
arr[3] = 60;  // Modifies the value of the fourth element (index 3)

// Accessing elements using a variable as an index
int index = 2;
int element = arr[index]; // Accesses the element at index 2 (third element)

// Be cautious to not access elements beyond the array bounds
// This may lead to undefined behavior

```

## Multi-dimensional arrays

In C++, you can create multi-dimensional arrays, which are essentially arrays of arrays. Here's how you can declare and initialize multi-dimensional arrays:

```cpp
// Syntax 1: Static multi-dimensional array
int matrix1[3][3] = {
    {1, 2, 3},  // Row 0
    {4, 5, 6},  // Row 1
    {7, 8, 9}   // Row 2
};

// Syntax 2: Dynamic multi-dimensional array (using pointers)
int **matrix2;
matrix2 = new int*[3]; // Allocate memory for rows
for (int i = 0; i < 3; ++i) {
    matrix2[i] = new int[3]; // Allocate memory for columns
}
// Initialize the array
matrix2[0][0] = 1;
matrix2[0][1] = 2;
// and so on...

// Syntax 3: Using std::array (requires C++11 or later)
#include <array>
std::array<std::array<int, 3>, 3> matrix3 = {{
    {1, 2, 3},  // Row 0
    {4, 5, 6},  // Row 1
    {7, 8, 9}   // Row 2
}};

```

- matrix1 is a static multi-dimensional array with dimensions 3x3. The size of the array is known at compile time.
- matrix2 is a dynamic multi-dimensional array created using pointers. Here, memory is allocated dynamically, allowing for more flexibility in array size.
- matrix3 is a multi-dimensional array using std::array from the C++ Standard Library. It offers some advantages over raw arrays, such as being able to use the at() member function for bounds-checking.

- When accessing elements of multi-dimensional arrays, you use multiple sets of square brackets. For example:

```cpp

int element = matrix1[1][2]; // Accesses the element at row 1, column 2

```

- Remember to manage memory properly, especially when using dynamic multi-dimensional arrays, to avoid memory leaks.

## String manipulation

In C++, string manipulation can be achieved using the standard library's `string` class, which provides a rich set of functions for working with strings. Here's an overview of common string manipulation operations:

1. **String Initialization and Assignment**:

   ```cpp

   #include <string>
   std::string str1 = "Hello";          // Initializing a string
   std::string str2 = str1;             // Copying a string
   std::string str3 = "World";          // Initializing another string

<!-- Concatenation: -->

std::string result = str1 + " " + str3;   // Concatenating strings

<!-- String Length: -->
int length = str1.length();           // Getting length of string

<!-- Accessing Characters: -->
char firstChar = str1[0];             // Accessing first character
char lastChar = str1.back();           // Accessing last character

<!-- Substring Extraction: -->
std::string substr = str1.substr(1, 3);  // Extracting substring from index 1 to 3

<!-- Searching: -->
size_t found = str1.find("lo");       // Searching for a substring
if (found != std::string::npos) {
    // Substring found
}

<!-- Replacing: -->
str1.replace(2, 2, "p");              // Replacing characters from index 2 with "p"

<!-- String Comparison: -->
if (str1 == str3) {
    // Strings are equal
}

<!-- Conversion: -->
int number = 123;
std::string strNumber = std::to_string(number);  // Converting int to string

These are just some of the basic string manipulation operations available in C++. The std::string class offers many more methods for various string-related tasks. Always remember to include the <string> header when working with strings in C++.

## Resources found on openAI
