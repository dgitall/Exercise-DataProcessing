# Exercise-DataProcessing
 
## Introduction
In the Data Processing lesson, we looked at some of the common issues you may encounter with real-world data sets. Now we'll get some hands-on practice finding and addressing these problems with Pandas and scikit-learn in Python.

## Files
Download the data set provided [here](https://stage3talent.brightspace.com/content/enforced/6771-Gen10DBC-21-10/M09/assets/files/ml-03-data-processing-songs-dataset.csv?_&d2lSessionVal=42tQ63oNvbEEAazL57FiW4iUX&ou=6771). Create a new notebook in Azure Machine Learning Studio for this exercise.

## Instructions
Read through the documentation below for guidance, then execute the following steps. Besides the methods specifically relevant to this lesson, you'll also need to recall some of the Pandas basics, documentation for which is included at the bottom of this page.

[Imputation of Missing Values](https://scikit-learn.org/stable/modules/impute.html)

[Time Series/Date Functionality](https://pandas.pydata.org/pandas-docs/stable/user_guide/timeseries.html)

[Pandas Get_Dummies](https://pandas.pydata.org/docs/reference/api/pandas.get_dummies.html)

[Preprocessing Data](https://scikit-learn.org/stable/modules/preprocessing.html)

1. Import the raw data set into a Pandas DataFrame. Perform some exploratory analysis on the raw data set. Check for the types of data hygiene issues mentioned in the lesson. Whenever you find a possible issue, write some code to fix it. Apply your fixes systematically, not case-by-case. Be sure to include comments to explain your process.
2. Find the number of missing values in each column and each row. Remove rows where at least 50% of the values are missing. Then remove columns where at least 50% of the values are missing.
3. Calculate descriptive statistics for each column. Let's define an outlier as a value at least 3 standard deviations away from the mean. Which columns have outliers? What are those values?
4. With the remaining columns, use scikit-learn to impute missing values. For continuous features, fill in the mean. For categorical features, fill in the mode.
5. Combine the date-related columns into one column with the Pandas to_datetime() method, then use that column to create a numeric Age column (in years). Calculate Age based on today's date; it doesn't have to be a whole number. Once you've created the Age column, remove the other date-related columns, including the one you created with Pandas.
6. Create dummy variables for the categorical features. Drop one level of each feature to end up with k-1 dummies, not k.
7. Save your work up to this point. Mark the end of this exercise in your notebook. If you have questions, reach out to an instructor.
## Additional Resources
[Pandas User Guide](https://pandas.pydata.org/docs/user_guide/index.html#user-guide) 

[Pandas DataFrame Reference](https://pandas.pydata.org/docs/reference/frame.html) 

[Pandas Series Reference](https://pandas.pydata.org/docs/reference/series.html) 

[Pandas loc Reference](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.loc.html) 

[Pandas iloc Reference](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.iloc.html) 