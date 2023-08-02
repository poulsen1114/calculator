# Simple Javascript Calculator

## Overview

This is a simple calculator app built with Javascript, HTML, and CSS. It allows the user to perform basic arithmetic operations like addition, subtraction, multiplication, and division.

## How to Use

- The calculator display starts at 0
- Click the number buttons to enter digits into the calculator display 
- Click an operator button (/, *, +, -) to choose an operator 
- Click the "=" button to get the result of the calculation
- Click the "C" button to clear the display and start new calculation
- Click the "." button to add a decimal point to the number

## Features

- Perform basic arithmetic operations
- Clear display with "C" button
- Chain together successive operations
- Handles decimals

## Code Overview

The core logic is handled in Javascript. 

### index.html

- Contains button elements for each digit, operator, and actions like clear
- Calculator display is a `<h1>` element
- Buttons have either a number class, operator class, or decimal class

### style.css

- Styles for digit buttons, operator buttons, and display

### calculator.js

- `calculatorDisplay` variable stores a reference to the display element
- `inputBtns` variable stores a NodeList of all number and operator buttons  
- `clearBtn` variable stores a reference to the clear button
- `calculate` object stores the operation functions for each operator
- `firstValue`, `operatorValue`, `awaitingNextValue` track the state of calculation  
- `sendNumberValue()` appends digits to the display or updates the display value
- `addDecimal()` appends a decimal point if needed
- `useOperator()` stores the first value and operator when pressed
- `resetAll()` clears all values and the display
- Event listeners call these functions for click events

## Possible Future Improvements

Some ways this calculator could be expanded on in the future:

- Support keyboard input of numbers and operators
- Support more complex operations like square root, exponents, etc
- Add memory features like "MC", "MR", etc
- Make the display scroll when the number gets very long rather than truncate
- Improve styling and visual design

Overall, this project demonstrates how to build a simple calculator app in Javascript and handle chained calculation logic.
