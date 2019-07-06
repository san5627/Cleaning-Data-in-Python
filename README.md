PART 1 - EXPLORING YOUR DATA

Cleaning Data : 
1. Prepare Data for Analysis
2. Data almost never comes in clean
3. Diagnose data for problems

Common Data problems :
1. Inconsistent column names
2. Missing Data
3. Outliers
4. Duplicated rows
5. Untidy
6. Need to process columms
7. Columns types can signal unexpected data values

Exploratory Data Analysis : 
1. Frequency Counts - Count the number of unique values in the data.
2. Summary Statistics
- Numeric columns (describe() which return only numeric values)
- Outliers - Considerably higher or lower, require further investigations

Visual EDA : 
- Great way to spot outliers and obvious errors
- More than just looking for patterns
- Plan data cleaning steps

Bar plots and histograms :
- Bar plots for discrete columns counts
- Histogram for continuous data counts
- Look at frequencies

Box plot : Visual basic summary statistics
- Outliers
- Min / Max
- 25th, 50th, 75th percentiles

Scatter plot :
- Relationship between 2 numeric variables
- Flag potentially bad data which we cannot look by looking at 1 variables


PART 2 - TIDYING DATA FOR ANALYSIS

Tidy Data :
- Formalize the way we describe the shape of Data
- Gives us a goal when format ting our data
- "Standard way to organize data values within a dataset"

3 principles of Tidy Data : 
1. Columns represent seperate variables
2. Rows represent individual observations
3. Observational unit forms tables

Pivot : Un-melting the Data : 
- Opposite of melting
- In melting, we turn columns into rows
- Pivoting : turn unique values into seperate columns
- Multiple variables stored in the same column


PART 3 - COMBINING DATA FOR ANALYSIS

- Data may not always come in 1 huge file
- 5 million row dataset may be broken into 5 seperate datasets'
- Easier to store and share
- May have new data for each day
- Important to be able to combine then clean or vice versa

Concatenating many files : 
- They must be in list
- Can individually load if there was a few datasets
- glob() to find files based on a pattern

Globbing :
- Pattern matching for file names
- Wildcards -  *? implies any .csv files or any single character: file_?.csv
- Return a ;ist of file names
- Can use this list to load into seperate DataFrames

Then the plan :
- Load files from globbing into pandas
- Add the dataframes into a list
- Concatenate multiple datasets at once

Combining Data in many ways : Use merging
- Type of Meger are
- One-to-one
- Many-to-one / one-to-many
- Many-to-many


PART 4 - CLEANING DATA FOR ANALYSIS

Data Types : 
- Use df.types() to see data types
- Convert using df['column_name'].astype(str)

Using regular expressions to clean strings : 
- String manipluation
- apply() to create new columns

Duplicated Data :
- Can skew results 
- '.drop_duplicates()' method

Missing Data : 
- NaN missing values
- Treatment like leave as it is, drop them or fill them

Assert Statements : 
- After all treatment, we expect no missing values
- In other word, if we drop or fill NaNs we expect zero missing values
- We can write an assert statement to verify this
- We can detect early warning and errors
