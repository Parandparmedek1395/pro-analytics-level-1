# Data Examples

[Professional Analytics](https://github.com/denisecase/pro-analytics)

## Table of Contents

- [CSV Examples](csv/)
- [HTML Examples](html/)
- [JSON Examples](json/)
- [Parquet Examples](parquet/)
- [Pickle Examples](pickle/)
- [SQLite Examples](sqlite/)
- [Text File Examples](txt/)
- [XLSX Examples](xlsx/)
- [YAML Examples](yaml/)

## Why This Topic is Important

Data analytics professionals need to be able to work with data in a variety of formats.

## Introduction

This folder provides examples of formats you might encounter.
Recognizing and working with multiple data formats is crucial for data analytics
professionals.

## Basic Text Formats

These formats are primarily used for simple text data.

### .csv (Comma-Separated Values File)

Various datasets suitable for machine learning tasks, ranging from simple to
complex structures.
Sources include:

- [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/index.php)
- [CSV Files](https://people.sc.fsu.edu/~jburkardt/data/csv/csv.html)
- [AdventureWorks](https://github.com/nuitsjp/AdventureWorks-for-SQLite/tree/master/Source)
- [Pandas Tutorial](https://github.com/LearnDataSci/articles/tree/master/Python%20Pandas%20Tutorial%20A%20Complete%20Introduction%20for%20Beginners)
- [Example: deniro.csv](./csv/deniro.csv)
- [Example: IMDB-Movie-Data.csv](./csv/IMDB-Movie-Data.csv)

### .txt (Text File)

Social media, classic literature texts, such as novels or poetry,
error messages, web content.
Typically unstructured information that can be used for text analysis,
natural language processing, or simple word frequency counts.
See [Working with Text Files](https://cs.brown.edu/courses/csci0112/fall-2020/lectures/working-with-text-files.html)
for more information.
Sources include:

- [Project Gutenberg](https://www.gutenberg.org/)
- [Frankenstein](https://www.gutenberg.org/files/84/84-0.txt)
- [Example: frankenstein.txt](./txt/frankenstein.txt)

## Structured Data Formats

These formats are used for data that has a specific structure or schema.

### .html (Hypertext Markup Language File)

An HTML page from a news website, blog, or Wikipedia, useful for web
scraping and data extraction.
Sources include:

- Extract from any informational website.
- Right-click on the page and select "View Page Source" to see the HTML code.
- [Wikipedia Analytics](https://en.wikipedia.org/wiki/Analytics)
- [Example: wikipedia-analytics.html](./html/wikipedia-analytics.html)

### .json (JavaScript Object Notation File)

Sample data format common in real or fake online REST API, like user posts or
comments are excellent for practicing JSON parsing and data manipulation.
See [Introduction to Using JSON With Data Analytics](https://bootcamp.berkeley.edu/resources/coding/learn-data-analytics/introduction-to-using-json-with-data-analytics/)
for more.
Sources include:

- [JSONPlaceholder](https://jsonplaceholder.typicode.com/)
- [Random ]

### .xlsx (Excel Spreadsheet)

Excel datasets may be related to economics, health, social sciences, sports,
and much more.
These often include multiple sheets and complex structures.
The structure is ideal for data cleaning and analysis.
Sources include:

- [Kaggle Datasets](https://www.kaggle.com/datasets)

## Advanced Data Formats

These formats are typically used in more advanced data processing and analysis.

### .db or .sqlite (Database File)

Simple file-based databases with tables often related to a business scenario,
like sales or inventory data.
Good for practicing SQL queries.
Sources include:

- Create your own using SQLite.
- [AdventureWorks](https://github.com/nuitsjp/AdventureWorks-for-SQLite/blob/master/Source/instawltdb.sql)

### .parquet (Apache Parquet File) also .parq

Not-human readable.
Parquet files are efficient for columnar storage and often used in big data processing.
They are compressed and can be partitioned,
making them ideal for data warehousing and analytics. Often used in data lakes.
Sources include:

- Create your own.
- [Apache Parquet Example Files](https://github.com/apache/parquet-testing)
- [Reading and Writing the Apache Parquet Format](https://arrow.apache.org/docs/python/parquet.html)
- [Example: parquet-nan_in_stats.parquet](./parquet/nan_in_stats.parquet)

### .pickle (Pickle File) also .pkl

Not-human readable. Pickle is used to serialize a Python object,
like a DataFrame or a machine learning model, for sending data across a network
or storing in a file.
Pickle takes a Python object and converts it to a string representation which
can be converted back into the original object.
Pickle is not secure.
Do not un-pickle untrusted content, as the file could contain malicious code.

Sources include:

- Create your own.
- [Pickle](https://docs.python.org/3/library/pickle.html)
- [Pickle Example](https://www.datacamp.com/community/tutorials/pickle-python-tutorial)

## Resources

- [Data File Formats](https://en.wikipedia.org/wiki/List_of_file_formats#Data_file_formats)
- [cURL command-line tool](https://curl.se/)
- [cURL command](https://everything.curl.dev/)
