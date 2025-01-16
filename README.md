# String Calculator TDD Kata

This project implements the **String Calculator TDD Kata**, a task designed to showcase Test-Driven Development (TDD) principles. The goal is to create a `StringCalculator` class that adheres to the requirements while following TDD best practices.

## Table of Contents

1. [Overview](#overview)
2. [Features](#features)
3. [Getting Started](#getting-started)
4. [Usage](#usage)
5. [Implementation Details](#implementation-details)
6. [Development Process](#development-process)
7. [Run Tests](#run-tests)
8. [Project Structure](#project-structure)
9. [Contributing](#contributing)
10. [License](#license)

---

## Overview

The **String Calculator TDD Kata** is a popular coding exercise that emphasizes:
- Writing code incrementally with tests.
- Refactoring after each passing test.
- Building a robust, testable, and maintainable solution.

### Requirements
1. Create a method `add(string numbers)` that:
   - Returns the sum of numbers in a string, separated by commas or newlines.
   - Handles custom delimiters.
   - Throws exceptions for negative numbers and displays all negatives in the error message.

---

## Features

- **Sum Numbers**: Parses a string of numbers and returns their sum.
- **Custom Delimiters**: Allows custom delimiters like `;`, `|`, or others.
- **Exception Handling**: Throws errors for negative numbers with detailed messages.
- **Scalable**: Supports an arbitrary number of numbers as input.

---

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v16+ recommended)
- [NPM](https://www.npmjs.com/) (comes with Node.js)
  
## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/skrnagar/string-calculator-tdd-kata.git
   cd string-calculator-tdd-kata
2. Install dependencies:
   ```bash
   npm install

## Usage

### Example Usage

Use the `add` function in the `StringCalculator` class:

   ```javascript
   const StringCalculator = require('./src/StringCalculator');
   const calculator = new StringCalculator();
   
   console.log(calculator.add("1,2,3")); // Output: 6
   console.log(calculator.add("1\n2,3")); // Output: 6
   console.log(calculator.add("//;\n1;2")); // Output: 3
   ```

## Implementation Details

The `StringCalculator` implementation focuses on:
1. **Empty Strings**:
   - Input: `""`
   - Output: `0`
2. **Single Number**:
   - Input: `"1"`
   - Output: `1`
3. **Two Numbers**:
   - Input: `"1,2"`
   - Output: `3`
4. **Unknown Count of Numbers**:
   - Input: `"1,2,3,4"`
   - Output: `10`
5. **Newline Delimiters**:
   - Input: `"1\n2,3"`
   - Output: `6`
6. **Custom Delimiters**:
   - Input: `"//;\n1;2"`
   - Output: `3`
7. **Negative Numbers**:
   - Input: `"1,-2,-3"`
   - Output: Exception: `Negative numbers not allowed: -2, -3`

---

## Development Process

The project follows the Test-Driven Development (TDD) process:
1. Write a failing test.
2. Write minimal code to pass the test.
3. Refactor for clarity and performance.

## Run Tests

1. Run tests using the following command:
   ```bash
   npm test
2.	Test Framework: Jest

## Example Output

PASS  tests/StringCalculator.test.js
✓ Should return 0 for an empty string
✓ Should return the number for a single number
✓ Should return the sum of two numbers
✓ Should handle multiple numbers
✓ Should handle newlines as delimiters
✓ Should handle custom delimiters
✓ Should throw an exception for negative numbers

## License

This project is open-source and available under the MIT License.

## Author

Sunil Kumar Nagar
Contact: skngrp@gmail.com
GitHub: https://github.com/skrnagar

This completes the **Development Process** and **Run Tests** sections in your `README.md` file.
Save this content as `README.md` in your project. It includes all the requested sections and a comprehensive structure for your documentation.


   
