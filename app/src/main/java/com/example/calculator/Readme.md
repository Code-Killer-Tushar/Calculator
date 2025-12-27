# Calculator App (Jetpack Compose)

A simple Android calculator application built using **Jetpack Compose**.  
This app supports basic arithmetic operations with a clean UI and light/dark theme support.

---

## Features

- Basic operations: **Addition (+), Subtraction (-), Multiplication (x), Division (÷)**
- Decimal number support
- Clear all (`AC`) and backspace (`⌫`) functionality
- Prevents multiple operators in a single expression
- Removes unnecessary `.0` from results
- Automatically adapts to **system light/dark theme**
- Modern UI built entirely with **Jetpack Compose**

---

## Tech Stack

- **Language:** Kotlin
- **UI Toolkit:** Jetpack Compose
- **Architecture:** State-based UI using `remember` and `mutableStateOf`
- **Minimum Android Version:** Compatible with modern Android versions supporting Compose

---

## How It Works

- User input is stored in a single `screen` state variable.
- Only one operator is allowed at a time.
- The `result()` function:
    - Detects the operator
    - Splits operands
    - Performs the calculation
    - Returns a `Double` result
- The result is formatted to remove trailing `.0` when not needed.

---

## Supported Operations

| Operator | Description |
|--------|-------------|
| `+` | Addition |
| `-` | Subtraction |
| `x` | Multiplication |
| `÷` | Division |

---

## UI Highlights

- Responsive button layout using `Row` and `Column`
- Large, readable text for numbers and results
- Color-coded operator buttons
- Dynamic background based on system theme

---

## Limitations

- Supports only **single-operation expressions** (e.g., `12 + 5`)
- No parentheses or advanced math functions
- No error handling for division by zero (can be added)

---

## Future Improvements

- Support for multi-step expressions
- History of calculations
- Scientific calculator mode
- Better input validation and error handling

---

## Author

**Tushar Biswas**  
Android Developer

---

## License

This project is for learning and portfolio purposes.
