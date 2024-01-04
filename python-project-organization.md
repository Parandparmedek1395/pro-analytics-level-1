# Python Organization

## Why This Topic is Important

We need to know how projects are built.

## Variable

A name that refers to a value.

## Expression

A combination of values, variables, and operators.

## Statement

A unit of code that has an effect, like creating a variable or displaying a value.

## Function

A named sequence of statements that performs some useful operation.
Functions may or may not take arguments and may or may not produce a result.

## Class (Optional)

Some Python projects use classes, but not all.
A data analyst needs to know when this would be a useful way to organize code.
Use a class when data and functions are closely related.
A class is a collection of functions and variables that are used to create objects.
Class data fields are called attributes.
Class functions are called methods.

For example, when working with veterinary records, we might have a class for animals.
Each animal would have a name, age, and weight.
We could have sub-classes for dogs, cats, and birds,
 each with their own unique attributes and methods.

Common Python classes for analytics include **pandas.DataFrame** and sklearn.linear_model.LinearRegression.
when we want to work with tabular data, we create a DataFrame object.
When we want to create a linear regression model, we create a LinearRegression object.
We then use the methods to gain insights from the data.

## Object

An object is an instance of a class.

## File / Module / Script

A file is a collection of related functions and classes.
A Python file has a .py extension.
A module is a Python file that can be imported into another file.
A script is a Python file that can be run directly.

## Package

A package is a collection of related modules.

## Library

A library is a collection of related packages. For example:

- The Python Standard Library
- The Pandas library
- The Scikit-learn library
- The Matplotlib library
- The Seaborn library

## Distribution

A distribution is a collection of related libraries and packages. For example:

- Anaconda distribution
- Miniconda distribution

## Project

A project is a collection of related files, modules, and packages
that work together for a specific purpose.
