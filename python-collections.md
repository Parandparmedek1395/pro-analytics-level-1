# Python Collection Data Types

[Professional Analytics](https://github.com/denisecase/pro-analytics)

## Why This Topic is Important

Collections are like containers where you can store and organize data.
Each collection type has its own unique features and uses, making it important to know which one to use and when. Mastering these types not only helps you write more efficient and organized code but also opens up a world of possibilities in data manipulation and analysis.

## Introduction

Python offers several built-in collection data types, each with unique characteristics.
These collections help you manage and operate on data effectively. Here’s a quick guide:

### Indexes - Start at 0

- In Python, indexing starts at 0, meaning the first element of any collection is accessed at index 0.

### Range - Start at 0, Stop before the End

- Use the `range()` function to generate a sequence of numbers.
- Includes the start number
- Up to, but not including the end number
- Returns a range object (not a list)
- Typically, the result is converted to a list using list() or []

### String Operations and Slicing

- Strings in Python can be manipulated and sliced using indexing and slicing techniques, allowing you to extract and modify sub-parts of a string.
- Strings are immutable, meaning they cannot be changed in-place.
- To modify a string, you must create a new string with the desired changes.
- Strings can be concatenated using the `+` operator.
- Strings can be repeated using the `*` operator.
- Strings can be sliced using the `[]` operator,
- Slicing syntax: `string[start:stop:step]`, e.g. `greeting[0:5:2]` returns every other character from the first five characters of the string.

### List

- Lists are ordered and changeable collections that allow duplicate members.
- They are great for storing an **ordered sequence** of items.

### Tuple (Like a Record or Row in Excel or a Database)

- Tuples are ordered and unchangeable collections.
- Tuples are perfect for grouping related data that should not be modified.

### Dictionary (Labeled Data)

- Dictionaries are unordered, changeable, and indexed collections with no duplicate members.
- Dictionaries store data in key-value pairs and are excellent for fast data lookups.
- Very similar to the JSON data format.

### Set

- Sets are unordered and un-indexed collections with no duplicate elements.
- Sets store unique items and perform set operations like unions and intersections.

## Resources

[7:42:06 String Operations](https://www.youtube.com/watch?v=1PAy6d16ADQ&t=27726s)
[7:46:04 Lists and Tuples](https://www.youtube.com/watch?v=1PAy6d16ADQ&t=27964s)
[7:54:56 Dictionaries](https://www.youtube.com/watch?v=1PAy6d16ADQ&t=28496s)
[7:57:21 Sets](https://www.youtube.com/watch?v=1PAy6d16ADQ&t=28641s)
