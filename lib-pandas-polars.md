# Python Libraries: Pandas and Polars

[Professional Analytics](https://github.com/denisecase/pro-analytics)

## Why This Topic is Important

Pandas and Polars are popular libraries for handling data in Python.
Pandas is built on Numpy, and they are often used together.
Polars is a newer Rust-based library faster than Pandas for many operations.

## Introduction

Both provide a DataFrame class for working with data in a tabular format, e.g., spreadsheets.

## DataFrames

Both Pandas and Polars provide a DataFrame class for working with tabular data.

- **DataFrame**: A two-dimensional tabular data structure with labeled axes.

## Data Loading

Pandas (many formats):

- `pd.read_csv()`
- `pd.read_excel()`
- `pd.read_sql()`

Polars (smaller set):

- `pl.read_csv()`
- `pl.read_parquet()`

## Data Inspection

Pandas:

- `df.head()`, `df.tail()`, `df.describe()`, `df.info()` for inspecting the first/last rows, summary statistics, and information about the DataFrame.

Polars:

- `df.head()`, `df.tail()`, `df.describe()`, `df.schema()` for similar purposes.
 The methods are quite parallel, with minor differences in output details.

## Data Manipulation

Pandas:

- Column addition: `df['new_col'] = values`
- Column deletion: `df.drop(columns=['col'])`
- Filtering: `df[df['col'] > value]`
- Group by: `df.groupby('col').agg({'col2': 'sum'})`

Polars:

- Column addition: `df.with_column(pl.col('existing_col') * 2)`
- Column deletion: `df.drop('col')`
- Filtering: `df.filter(pl.col('col') > value)`
- Group by: `df.groupby('col').agg(pl.col('col2').sum())`

## Join Operations

Pandas:

- `df1.merge(df2, on='key', how='left/right/inner/outer')` for SQL-like join operations.

Polars:

- `df1.join(df2, on='key', how='left/right/inner/outer')` for SQL-like join operations.

## Performance

Pandas:

- Pandas operations are generally single-threaded and can be slower on large datasets.

Polars:

- Polars is designed for speed.
- Can automatically use multiple cores for many operations.
- Enabling faster performance on large datasets.

## Memory Usage

Pandas:

- Can be memory-intensive, especially when loading large datasets or chaining operations that create copies of the DataFrame.

Polars:

- More efficient memory usage due to columnar storage format and optimizations for large datasets.

## Unique and Specific Features

Pandas:

- Rich support for time series data and operations.
- More extensive visualization integration directly from DataFrame methods.

Polars:

- Lazy evaluation (using `pl.LazyFrame`) allows for optimization of operations before execution, which can significantly improve performance.
- Expression system that allows complex operations to be defined more succinctly.

## See Also

Both are often used with:

- **Matplotlib**: Plotting library for creating static, animated, and interactive visualizations.
- **Seaborn**: Data visualization library based on Matplotlib.
- **Plotly**: Graphing library for making interactive, publication-quality graphs online.

## Resources

- [Pandas](https://pandas.pydata.org/)
- [Polars](https://pola.rs/)
