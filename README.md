# Fundamental code concepts

This file contains some of the fundamental code concepts that beginners should try to understand as they start learning to code. There are other important concepts, but I have selected those that I feel are most relevant and important for beginners.

- [Variables and Data Types](#variables-and-data-types)
  - [Naming conventions](#naming-conventions)
  - [Syntax](#syntax)
  - [Comments](#comments)
- [Control Flow](#control-flow)
- [Functions](#functions)
- [Debugging](#debugging)
- [Error Handling](#error-handling)
- [Version Control](#version-control)
- [Algorithmic Thinking](#algorithmic-thinking)
  - [Problem Decomposition](#problem-decomposition)
  - [Logical Sequence](#logical-sequence)
  - [Patterns and Abstractions](#patterns-and-abstractions)
  - [Efficiency and Optimization](#efficiency-and-optimization)
  - [Iterative Problem Solving](#iterative-problem-solving)

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

Regarding style it is best practice to choose one and stick to it within a project.

Consistency makes code more easily read and understood.

### Syntax

In programming, **syntax refers to the set of rules governing the structure of code in a particular language**. It encompasses conventions for punctuation, spacing, and the arrangement of elements. Understanding and adhering to the syntax of a programming language is crucial for writing valid and functional code.

Each programming language has its own syntax rules, which may include requirements for line endings, the use of commas or semicolons, and conventions for indentation. Additionally, languages may have specific rules regarding variable and function declarations, initializations, and calls.

A solid grasp of syntax ensures that your code is not only readable but also interpretable by the compiler or interpreter.

### Comments

In programming, most languages offer a mechanism for incorporating human-readable text that is not considered part of the executable code. These are known as **comments**.

While it is considered a best practice to craft code with self-explanatory and meaningful names, there are instances where comments become necessary to elucidate certain aspects of the code.

In rare cases, you may find it beneficial or even essential to include comments for the following purposes:

- Inline comments: Clarify complex code snippets or offer additional context with comments placed directly within the code.
- Header comments: Integrate comments at the commencement of functions or sections to provide a concise description of their intended purpose.

While the goal is to make code as self-explanatory as possible through meaningful naming conventions and clear structure, judicious use of comments can enhance code readability, especially in scenarios where the logic might be intricate or the purpose of a particular block of code is not immediately evident. Striking a balance between expressive code and insightful comments contributes to the overall maintainability and collaborative nature of the codebase.

## Control Flow

In programming, **control flow** refers to **the order in which instructions are executed in a program**. It determines the path that the program takes based on conditions and loops. Understanding control flow is **essential for creating logical and functional programs**.

**Conditional statements allow the program to make decisions** and execute different blocks of code **based on certain conditions**. In Python, `if`, `else` and `elif` (else if) statements are available for the program to make decisions.

**Loops enable the repetition of a block** of code until a certain condition is met. In Python, 2 common types include the `for` and `while` loops.

## Functions

In programming, **functions** (or methods, depending on the terminology of the programming language) are essential **building blocks** that **encapsulate a specific task or set of tasks**. They play a vital role in promoting code organization, reusability, and modular design, serving as reusable pieces of code with specific purposes.

It is best practice to create functions that do only one thing, if at all possible. It is better for code readability and maintainability to have many smaller functions with descriptive names, than to have one complex and long function that does many things.

Like variables, **functions need to be declared**. Declaring a function involves specifying its name, parameters (if any), and the actions it performs. Functions often use the `return` statement to send a value back to the calling code. This returned value can be stored in a variable for further use.

To **execute a function** and make it perform its defined actions, **you need to call it** with specific arguments, corresponding to the required parameters.

**The difference between parameters and arguments**:
- Parameters: These are variables in the function declaration that act as placeholders for the values that will be passed into the function.
- Arguments: These are the actual values that are passed into the function when it is called.

Variables defined within a function are typically scoped to that function, meaning they are only accessible from within that function. Conversely, variables defined outside of a function are typically scoped within the file or block they are declared within.

Many programming languages come with **built-in functions that perform common tasks**. For example, in Python, `len()` is a built-in function that returns the length of a sequence.

## Debugging

When the code we write does not perform as we expect it to, bugs or errors may be present in the code. These issues can stem from incorrect logic, flawed implementation, or other factors.

**Debugging** is the skill that **enables you to identify and fix errors or bugs** in your code. It is a skill that aids in the creation of functioning, robust, and reusable code.

Here are key principles of effective debugging:

1. Error Identification:

    - Understand error messages: Read error messages carefully to pinpoint the issue.
    - Use debugging tools: Leverage integrated development environment (IDE) tools or external debuggers to step through your code.
2. Isolation and Reproduction:

    - Isolate the problem: Narrow down the portion of code causing the issue.
    - Create minimal examples: Simplify the code to create a small, reproducible test case.
3. Print Statements and Logging:

    - Use print statements: Insert print statements strategically to output variable values and trace program flow.
    - Logging: Implement logging to record events, making it easier to trace the program's execution.
4. Interactive Debugging:

    - Set breakpoints: Pause the execution of your code at specific points to inspect variables and step through the code.
    - Interactive consoles: Utilize interactive consoles available in IDEs to test code snippets.
5. Documentation Reading:

    - Consult documentation: Read the documentation for libraries and frameworks you are using to understand their behavior.
    - Online resources: Explore forums, communities, and Q&A websites for solutions to common issues.

## Error Handling

**Error handling involves managing and addressing unexpected issues or exceptions in your code**. Proper error handling enhances the **robustness** of your programs and provides a **better user experience**.

**Exceptions** are **unexpected events or errors** that can occur **during program execution**. Different programming languages have various types of exceptions, each representing a specific error condition.

Exceptions are most commonly handled by `try-except` blocks to encapsulate code that might raise an exception. The try block contains the code you want to execute. When an exception is raised, it can then be caught and handled gracefully by the except block, which contains the code to execute when an exception occurs. The except block should display informative error messages to aid in troubleshooting i.e. what went wrong and, possibly, potential solutions.

Once exception handling is implemented, **unit tests can** be implemented to **verify that error-handling mechanisms work as intended**.

## Version Control

**Version Control is a system that records changes to files over time**, enabling you to recall specific versions later. It provides a systematic way to track revisions, collaborate with others, and roll back to previous states when needed.

It will serve you well to learn to use a version control system, like [Git](https://git-scm.com/).

A version control repository is a central database that stores all changes made to the codebase.

**Best Practices**:

- Commit Frequently: Make small, logical commits to make tracking changes more manageable.
- Meaningful Commit Messages: Write descriptive commit messages to convey the purpose of each change.
- Branch Strategy: Adopt a branching strategy that fits your project's needs.

## Algorithmic Thinking

**Algorithmic thinking** is a a problem-solving mindset applicable to various fields, and is a fundamental skill in programming. It involves solving problems methodically and logically, and is all **about breaking down complex tasks into a series of step-by-step instructions**, or algorithms, that a computer can understand and execute.

### Problem Decomposition

Identify the Problem: Clearly define the problem you need to solve.

Break It Down: Divide the problem into smaller, more manageable sub-problems. This makes it easier to tackle each part individually.

### Logical Sequence

Define Steps: For each sub-problem, outline a logical sequence of steps or actions. Think about the order in which these steps should be executed.

Consider Dependencies: Understand dependencies between different steps. Ensure that the output of one step is suitable input for the next.

### Patterns and Abstractions

Recognize Patterns: Look for recurring patterns or similarities in the problems you encounter. Reusing solutions or algorithms for similar patterns can save time.

Abstraction: Abstract the problem to its essential components, ignoring unnecessary details. Focus on the core logic and steps needed to solve the problem.

### Efficiency and Optimization

Evaluate Complexity: Consider the time and space complexity of your algorithm. Aim for solutions that are efficient in terms of both time and resources.

Optimize: Seek ways to improve the algorithm's performance without sacrificing correctness. This may involve refining steps, using more efficient data structures, or finding alternative approaches.

### Iterative Problem Solving

Test and Refine: Implement your algorithm and test it with various inputs. Refine the solution based on testing outcomes.

Iterate: If needed, iterate through the process, refining and optimizing until you achieve a satisfactory solution.
