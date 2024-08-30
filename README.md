# Python to C++ Compiler

Welcome to the Python to C++ Compiler project! This project aims to convert Python code into equivalent C++ code through various stages, including lexing, parsing, semantic analysis, optimization, and code generation. The first component of this project is the lexer, which tokenizes Python code into its basic components.

## Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Lexer](#lexer)
- [Parser (Coming Soon)](#parser-coming-soon)
- [Semantic Analyzer (Coming Soon)](#semantic-analyzer-coming-soon)
- [Code Optimizer (Coming Soon)](#code-optimizer-coming-soon)
- [Code Generator (Coming Soon)](#code-generator-coming-soon)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

The Python to C++ Compiler project is designed to take Python code as input and convert it into equivalent C++ code. This project is useful for educational purposes, cross-compilation, or simply understanding how Python constructs can be translated into C++.

### Stages of Compilation

1. **Lexical Analysis (Lexer)**: Breaks down Python code into tokens.
2. **Syntax Analysis (Parser)**: Analyzes tokens according to Python grammar.
3. **Semantic Analysis**: Checks for semantic errors and ensures logical correctness.
4. **Optimization**: Improves code performance and efficiency.
5. **Code Generation**: Translates Python code into C++ code.

## Features

- **Tokenization of Python Code**: The lexer converts Python code into tokens, identifying keywords, identifiers, literals, operators, and other symbols.
- **Extendable Framework**: Easily add more tokens or expand the capabilities to cover more Python features.
- **Error Handling**: Detects and reports errors at the lexical level.

## Installation

To set up the project locally, follow these steps:

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/yourusername/python-to-cpp-compiler.git
    cd python-to-cpp-compiler
    ```

2. **Set Up a Virtual Environment** (Optional but recommended):
    ```bash
    python3 -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3. **Install Dependencies**:
    The project currently doesn't have any external dependencies, but you can add them to a `requirements.txt` file if needed.

## Usage

To run the lexer on a sample Python script:

1. **Create a Python file** (e.g., `example.py`) with some code:
    ```python
    x = 42
    y = x + 5
    name = "Alice"
    if x < y:
        print(name)
    ```

2. **Run the Lexer**:
    ```bash
    python lexer.py example.py
    ```

   This will output the tokens found in `example.py`.

## Lexer

The lexer is the first stage of the compiler, responsible for breaking down Python code into meaningful tokens.

### How It Works

- **Token Definition**: The lexer uses regular expressions to define tokens such as numbers, strings, identifiers, operators, and keywords.
- **Tokenization**: It processes the input Python code and generates a list of tokens.
- **Error Handling**: Any unexpected characters are reported as errors.

### Example

The following Python code:
```python
x = 42
name = "Alice"
if x < 50:
    print(name)