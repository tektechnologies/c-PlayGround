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


- Multi-dimensional arrays
- String manipulation

## Resources found on openAI
