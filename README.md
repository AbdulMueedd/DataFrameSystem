# DataFrameSystem
DataFrame System,You write your own way to store a table (rows and columns) of data (a DataFrame) and perform some basic statistical operations and sub-setting on the data. Users can load a DataFrame using a CSV (comma-separated values) file and also save a manipulated (subset) DataFrame in a new CSV. 

DataFrame - Has a collection of column headers, a collection of datatypes for each column (int double char String), and a collection of data rows (max size 25,000 rows). You use polymorphism to be able to store data of different types in the same collection of rows. Any errors in DataFrame methods should throw an exception, and when caught the details of the exception should be written to a log.txt file. Other than the method to write out the active DataFrame to a CSV file (using the name of the DataFrame as the name of the CSV file), the DataFrame class should not do any file reading or writing. Instead the DataFrameMenu should handle all other file reading/writing.

DataFrameMenu - The user interface (void main) to allow a user to create and analyze DataFrames (up to 10 loaded at a time). Any exceptions thrown from a DataFrame should be handled and logged in a log.txt file. The active DataFrame is the one that commands execute on. This functionality is required:
●	import a valid CSV, create a DataFrame, and make it the active DataFrame
●	change the active DataFrame to one loaded already
●	average a column in the active DataFrame, only works on numeric columns, given a column name for numeric data, return the average of the values in the column (if any error in method, return Double.NaN)
●	find the minimum of a column in the active DataFrame, only works on numeric columns, given a column name for numeric data, return the minimum of the values in the column (if any error in method, return Double.POSITIVE_INFINITY)
●	find the maximum of a column in the active DataFrame, only works on numeric columns, given a column name for numeric data, return the maximum of the values in the column (if any error in method, return Double.NEGATIVE_INFINITY)
●	create a frequency table (5 equally sized intervals) of a column in the active DataFrame, only works on numeric columns (if any error in method, throw an exception)
●	subset a DataFrame - create a new DataFrame (and make it the new active one) from the current active DataFrame by selecting rows where "columnData operator value" boolean statement is true for the data in a column. The allowed operators are <  ==  >  != (if any error in method, throw an exception). Name the new DataFrame using the current DataFrame name along with the boolean statement.
●	export the active DataFrame to a CSV file named with the same name as the DataFrame. Include column names and data types in the first two rows.
●	quit


Each non "void main" class needs its own individual test program. Each non "void main" class needs its own individual exception class and should throw exceptions for any invalid action. Other classes need to catch these exceptions where appropriate and write out details to log.txt.

Code
1.	DataFrame System functionality
a.	Menu System
b.	import a valid CSV
c.	change the active DataFrame
d.	average a column
e.	minimum of a column
f.	maximum of a column
g.	frequency table
h.	subset a DataFrame
i.	export a DataFrame
2.	Test programs for each non "void main" class
3.	Exception classes implemented for each non "void main" class

