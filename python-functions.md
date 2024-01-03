# Python Functions

[Professional Analytics](https://github.com/denisecase/pro-analytics)

## Why This Topic is Important

When we write code, we write instructions. We want our instructions to be organized and we want to avoid repeating the same instructions multiple times.
We want to wrap up a particular set of instructions and give it a name.
The general term for this is a function.
We define the logic of the function once, and then we can call the function as many times as we want.

## Introduction

Functions are the primary building blocks of code.
They enable reuse and less us create complex projects out of small, reusable blocks of code.
We'll talk about calling functions, and then look at how we can define and call functions specific to our project.

## Skills

### Calling Built-in Functions

- Understand functions
- Call built-in functions
- Understand function arguments
- Understand function return values

### Defining Custom Functions

- Define custom functions
- State clearly the desired return value of the function.
- If no return value, describe the side effects of the function.
- State clearly the parameters of the function.
- How many parameters? What type?
- What is the purpose of the parameter?
- Is the parameter optional? If so, what is the default value?
- Is the parameter named? If so, what is the name?
- If not named, what is the order of the parameters?
- What is the purpose of the function?

### Defining Custom Functions with Type Hints

- Understand type hints
- Use type hints for function return value.
- Use type hints for function parameters

### Defining Custom Functions Using AI Assistants

- Many analysts use AI assistants to help them write good functions.
- The analyst must understand the problem and the solution.
- The analyst must clearly state the name, purpose, return value and the parameters of the function.
- The analyst will work with an AI assistant to write the function.
- The analyst will provide test values, called arguments, and will test the function to ensure correct behavior.
- The analyst will ensure the function is properly documented using docstrings and best practices.

## Define a Function

- Use the `def` keyword to define a function.
- Provide a clear name for the function, using Python standard snake_case for the name.
- Specify each parameter (provided value) the function needs.
- Indicate if the function is expected to return a value and the type of the return value.
- Indicate if any parameters are optional and provide a default value.
- Indicate if any parameters are named and provide the name.
- Include a colon at the end of the signature (first line) of the function definition.
- Indent the body of the function.
- Resume regular indentation when the function body has been written.

## Additional Keywords

- Use the `return` keyword to return a value from a function.
- Use the `pass` keyword to define a function that does nothing.
- Use the `None` keyword to return nothing from a function.
- Use the `global` keyword to access a global variable from within a function.

## Scope

- Understand scope
- Understand global scope
- Understand local scope

## Best Practices

## Best Practices in Function Design

- **Single Responsibility**: Each function should perform one specific task or responsibility.
- **Short and Concise**: Keep functions short. A function should fit on a single screen (around 10-20 lines).
- **Explicit Arguments**: Pass in everything the function needs as arguments, rather than relying on global variables.
- **Immutable Arguments**: Avoid mutating arguments passed to the function unless absolutely necessary. Prefer returning new values over modifying input values.
- **Clarity in Naming**: Choose clear and descriptive names for functions and their parameters, reflecting their purpose and usage.
- **Limit Parameter Count**: Keep the number of parameters as low as possible. If a function requires many parameters, it might be doing too much. If all parameters are related, group them into a single structure.
- **Document**: Use docstrings to document the purpose, parameters, return values, and all side effects of the function.
- **Error Handling**: Incorporate error handling within functions to manage potential exceptions.
- **Testing**: Write tests for your functions to ensure they behave as expected and handle edge cases.
- **Consistent Style**: Follow consistent coding styles and conventions for readability and maintainability.
- **Avoid Side Effects**: Functions should, ideally, not have side effects (unexpected changes to the program's state). They should depend only on their inputs and produce outputs or changes in state that are predictable from those inputs.

Following these guidelines will make your code much easier to test and maintain.
