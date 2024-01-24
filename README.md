# Fundamental code concepts

## Variables and Data Types

In computer science, **data** refers to **information that is meaningful to the computer**.

Programming languages **organize data** into distinct **data types**, and adherence to these types is crucial in many programming languages and in programming logic as various data types may behave differently within the same logic.

**Variables** serve as **containers for storing data** that have an associated label for easy access to the data. To be considered a variable, variables must be declared and then initialized. To be considered a variable, it must be declared and then initialized. This process is sometimes done in a single step; for example, in Python: `int count = 0;`. Declaring a variable is the process of introducing it to the compiler or interpreter, providing information about the variable's name and data type, in Python `int count;`. This step reserves a location in the computer's memory for the variable. Initialization is the subsequent step where you assign an initial value to the declared variable, as seen in Python: `count = 0;`. Until a variable is initialized, its content is considered undefined or garbage.
Until a variable is initialized, its content is considered undefined or garbage.
Essentially, variables enable computers to dynamically store and manipulate data by associating a "label" with the data rather than directly handling the data itself. The nature of what is stored—whether it is the location of other data or the actual value—varies depending on the programming language and data type.

### Naming conventions

Spaces or whitespace in names (file names, folder names, variable names etc.) can be difficult and inconvenient to handle in programming. Therefore, programmers often use one of the following casings to avoid the usage of spaces:

- `camelCase`
- `PascalCase`
- `lowercase_snake_case`
- `UPPERCASE_SNAKE_CASE`
- `kebab-case`

## Control Flow

In programming, **control flow** refers to **the order in which instructions are executed in a program**. It determines the path that the program takes based on conditions and loops. Understanding control flow is **essential for creating logical and functional programs**.

**Conditional statements allow the program to make decisions** and execute different blocks of code **based on certain conditions**. In Python, `if`, `else` and `elif` (else if) statements are available for the program to make decisions.

**Loops enable the repetition of a block** of code until a certain condition is met. In Python, 2 common types include the `for` and `while` loops.

## Functions

In programming, **functions** (or methods, depending on the terminology of the programming language) are essential **building blocks** that **encapsulate a specific task or set of tasks**. They play a vital role in promoting code organization, reusability, and modular design, serving as reusable pieces of code with specific purposes.

Like variables, **functions need to be declared**. Declaring a function involves specifying its name, parameters (if any), and the actions it performs. Functions often use the `return` statement to send a value back to the calling code. This returned value can be stored in a variable for further use.

To **execute a function** and make it perform its defined actions, **you need to call it** with specific arguments, corresponding to the required parameters.

**The difference between parameters and arguments**:
- Parameters: These are variables in the function declaration that act as placeholders for the values that will be passed into the function.
- Arguments: These are the actual values that are passed into the function when it is called.

Variables defined within a function are typically scoped to that function, meaning they are only accessible from within that function. Conversely, variables defined outside of a function are typically scoped within the file or block they are declared within.

Many programming languages come with **built-in functions that perform common tasks**. For example, in Python, `len()` is a built-in function that returns the length of a sequence.
