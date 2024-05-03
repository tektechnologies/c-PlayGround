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

- Accessing array elements
- Multi-dimensional arrays
- String manipulation

## Resources found on openAI
