# Data Cleaning

[Professional Analytics](https://github.com/denisecase/pro-analytics)

## Why This Topic is Important

Real data is messy. Much is too messy to be useful.
Cleaning the data is the process of preparing it for analysis.
It is a critical step in the data analytics process to ensure accuracy and reliability in analysis.

## Introduction

Data cleaning is a critical step in the data analytics process to ensure accuracy and reliability in analysis. This cheat sheet covers common techniques and best practices for cleaning data.

## General Principles

- **Consistency**: Ensure data is consistent across records and fields.
- **Accuracy**: Verify data is correct and remove or correct inaccuracies.
- **Completeness**: Fill in missing values where possible, or identify and handle them appropriately.
- **Validity**: Ensure data conforms to the expected format and range.

## Common Data Cleaning Techniques

### Dealing with Missing Values

- **Imputation**: Fill missing values with mean, median, or mode.
- **Deletion**: Remove records with missing values when they are insignificant.

### Handling Outliers

- **Identification**: Use statistical methods like IQR or Z-scores to identify outliers.
- **Treatment**: Cap, transform, or remove outliers based on the context.

### Data Transformation

- **Normalization**: Scale data to a small range, like 0-1.
- **Standardization**: Transform data to have a mean of 0 and standard deviation of 1.

### Data Type Conversion

- **Categorical to Numeric**: Convert categories to numbers for analysis.
- **Date Time Conversion**: Standardize and parse date-time formats for consistency.

### String Manipulation

- **Trimming**: Remove unnecessary spaces from strings.
- **Pattern Extraction**: Use regular expressions to extract information.

### Deduplication

- **Identify Duplicates**: Find and review duplicate entries.
- **Remove Duplicates**: Keep one copy of a duplicate record and remove the rest.

## Python Libraries for Data Cleaning

- **Pandas**: For data manipulation and cleaning.
- **NumPy**: For numerical operations.
- **SciPy**: For advanced scientific computing.
- **Scikit-learn**: For pre-processing and cleaning in machine learning workflows.

## Tips and Tricks

- **Automate Routine Tasks**: Use scripts to automate repetitive cleaning tasks.
- **Document the Process**: Keep a record of cleaning steps for reproducibility.
- **Visual Inspection**: Use plots and charts to identify anomalies and patterns.
- **Regular Updates**: Keep cleaning strategies updated with evolving data patterns.
