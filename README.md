
---

# Basics README

## Introduction

This C++ code provides a collection of utility functions for various text and user interaction tasks. These functions can be used to manipulate and work with strings, create user menus, clear the console screen, and perform other useful operations.

## Functions

### `lowercaseFirst`

This function takes a string as input and returns the same string with its first character converted to lowercase.

### `lowercaseAll`

Given a string, this function converts all characters (except spaces) to lowercase.

### `uppercaseAll`

This function, when given a string, converts all characters (except spaces) to uppercase.

### `uppercaseFirst`

Converts the first character of a string to uppercase and returns the modified string.

### `newLine`

Simply adds a newline to the console output.

### `clear`

Clears the console screen, providing a clean slate for the next output.

### `randomInt`

Generates a random integer within a specified range.

### `maxInput`

Compares an input value with a maximum value and returns the minimum of the two.

### `minInput`

Compares an input value with a minimum value and returns the maximum of the two.

### `wait`

Pauses the program for a specified amount of time (in seconds).

### `menuCreator`

Creates a menu by displaying a list of choices to the user and allowing them to select an option. Returns the index of the chosen option.

### `searchParam`

Converts a string to lowercase and replaces spaces with hyphens, useful for search parameter formatting.

## Usage

You can include this code in your C++ project to simplify common text manipulation and user interaction tasks. Here's a brief example of how to use some of these functions:

```cpp
#include <iostream>
#include "utility_functions.h"

using namespace std;

int main() {
    string input;
    cout << "Enter a string: ";
    cin >> input;

    string lowercased = lowercaseAll(input);
    cout << "Lowercased: " << lowercased << endl;

    string uppercased = uppercaseFirst(input);
    cout << "Uppercased First: " << uppercased << endl;

    clear();

    int randomNumber = randomInt(100);
    cout << "Random Number: " << randomNumber << endl;

    wait(2); // Wait for 2 seconds

    vector<string> choices = {"Option 1", "Option 2", "Option 3"};
    int choice = menuCreator(choices, "Select an option:");
    cout << "You chose: " << choices[choice - 1] << endl;

    return 0;
}
```

## License

This code is provided under the MIT License. You are free to use, modify, and distribute it as needed.

Please make sure to include the necessary header files and functions in your project for it to work correctly.

---

Feel free to customize this README to fit your specific project requirements, and make sure to provide information on how to integrate these utility functions into your code.
