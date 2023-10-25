# C++ Utility Functions

This repository contains a collection of utility functions written in C++ for various common tasks. These functions can be used to simplify and streamline your C++ programs. The included functions cover a range of tasks, from string manipulation to user interaction.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Functions](#functions)
  - [String Manipulation](#string-manipulation)
  - [User Interaction](#user-interaction)
- [Usage](#usage)

## Prerequisites

Before using these utility functions, you should have a C++ development environment set up. Ensure you have a C++ compiler (e.g., g++) installed on your system.

## Functions

### String Manipulation

#### `string lowercaseFirst(string input)`

This function converts the first character of a string to lowercase and returns the modified string.

#### `string lowercaseAll(string input)`

Converts all characters in a string to lowercase and returns the modified string.

#### `string uppercaseAll(string input)`

Converts all characters in a string to uppercase and returns the modified string.

#### `string uppercaseFirst(string input)`

Converts the first character of a string to uppercase and returns the modified string.

### User Interaction

#### `void newLine()`

Prints a newline character, effectively creating a blank line in the console.

#### `void clear()`

Clears the console screen.

#### `int randomInt(int max)`

Generates a random integer between 1 and the specified maximum value.

#### `int maxInput(int input, int max)`

Ensures that the provided input does not exceed the specified maximum value.

#### `int minInput(int input, int min)`

Ensures that the provided input is at least as large as the specified minimum value.

#### `void wait(int timeToWait)`

Pauses the program's execution for the specified number of seconds.

#### `int menuCreator(vector<string> menuChoices, string prompt)`

Displays a menu to the user with the provided choices and returns the index of the selected choice. The user can input their choice based on the menu item's name.

#### `string searchParam(string input)`

Standardizes the input string by capitalizing the first letter and converting the rest of the characters to lowercase. This function is useful for normalizing user inputs.

## Usage

To use these utility functions in your C++ program, follow these steps:

1. Include the `utility_functions.h` header in your C++ source code file.

```cpp
#include "basics.h"
```

2. Call the desired utility functions from your code as needed.

Example:

```cpp
string userInput;
cout << "Enter a string: ";
cin >> userInput;

// Normalize user input
userInput = searchParam(userInput);

cout << "Normalized input: " << userInput << endl;
```

Feel free to incorporate these functions into your C++ programs to streamline common tasks and improve code readability.
