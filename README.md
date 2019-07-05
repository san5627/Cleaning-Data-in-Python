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


