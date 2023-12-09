# Pandas-Challenge

# Background
You are the new Chief Data Scientist for your city's school district. In this capacity, you'll be helping the school board and mayor make strategic decisions regarding future school budgets and priorities.

As a first task, you've been asked to analyze the district-wide standardized test results. You'll be given access to every student's math and reading scores, as well as various information on the schools they attend. Your task is to aggregate the data to showcase obvious trends in school performance.

# Before You Begin
1. Create a new repository for this project called pandas-challenge. Do not add this homework to an existing repository.
2. Clone the new repository to your computer.
3. Inside your local Git repository, create a folder for this homework assignment and name it PyCitySchools.
4. Add your Jupyter notebook to this folder. This will be the main script to run for analysis.
5. Push these changes to GitHub or GitLab.

# Instructions
Using Pandas and Jupyter Notebook, create a report that includes the following data. Your report must include a written description of at least two observable trends based on the data.

Hint: Check out the sample solution called PyCitySchools_starter.ipynb located in the .zip file to review the desired format for this assignment.

# District Summary
Perform the necessary calculations and then create a high-level snapshot of the district's key metrics in a DataFrame. Include the following:

* Total number of unique schools
* Total students
* Total budget
* Average math score
* Average reading score
* % passing math (the percentage of students who passed math)
* % passing reading (the percentage of students who passed reading)
* % overall passing (the percentage of students who passed math AND reading)

# School Summary
Perform the necessary calculations and then create a DataFrame that summarizes key metrics about each school. Include the following:

* School name
* School type
* Total students
* Total school budget
* Per student budget
* Average math score
* Average reading score
* % passing math (the percentage of students who passed math)
* % passing reading (the percentage of students who passed reading)
* % overall passing (the percentage of students who passed math AND reading)

# Highest-Performing Schools (by % Overall Passing)
Sort the schools by % Overall Passing in descending order and display the top 5 rows.
Save the results in a DataFrame called "top_schools".

# Lowest-Performing Schools (by % Overall Passing)
Sort the schools by % Overall Passing in ascending order and display the top 5 rows.
Save the results in a DataFrame called "bottom_schools".

# Math Scores by Grade
Perform the necessary calculations to create a DataFrame that lists the average math score for students of each grade level (9th, 10th, 11th, 12th) at each school.

# Reading Scores by Grade
Create a DataFrame that lists the average reading score for students of each grade level (9th, 10th, 11th, 12th) at each school.

# Scores by School Spending
Create a table that breaks down school performance based on average spending ranges (per student).
Use the code provided below to create four bins with reasonable cutoff values to group school spending.

![image](https://github.com/JesseOli100/Pandas-Challenge/assets/62526904/afc1429a-bbfa-4afa-b951-4cc701a21e3e)!

Use pd.cut to categorize spending based on the bins. Use the following code to then calculate mean scores per spending range.

![Snip20231106_2](https://github.com/JesseOli100/Pandas-Challenge/assets/62526904/b4213508-2b02-4990-9311-373d5be63e86)

Use the scores above to create a DataFrame called spending_summary.
Include the following metrics in the table:

* Average math score
* Average reading score
* % passing math (the percentage of students who passed math)
* % passing reading (the percentage of students who passed reading)
* % overall passing (the percentage of students who passed math AND reading)

# Scores by School Size
Use the following code to bin the per_school_summary.

![Snip20231106_3](https://github.com/JesseOli100/Pandas-Challenge/assets/62526904/285faa76-f96a-4386-a97f-50aa58c91083)

Use pd.cut on the "Total Students" column of the per_school_summary DataFrame.
Create a DataFrame called size_summary that breaks down school performance based on school size (small, medium, or large).

# Scores by School Type
Use the per_school_summary DataFrame from the previous step to create a new DataFrame called type_summary.
This new DataFrame should show school performance based on the "School Type".

# Sources 

• Help from TA Matthew Werth and other staff

• Met up w/ other students during study groups to hash out the code through what we have learned so far

• Used StackOverFlow and ChatGPT for issues on the code and/or to explain why certain pieces of the script were not running as intended

• The majority of how it works is explained on the comments within the code or is self-explanatory throughout the flow of the code 

# Final Notes

What is each set of code supposed to be doing/What is the overall purpose?

The purpose of the code is to manipulate the sections within the dataframe to gather meaningful information about all of the best performing and lowest performing schools within a district and get the averages per student of where they excel and where they lack behind. This information can be useful for a school board or parent board in order to gather more information about how schools are teaching their children and what can/ought to be done about the quality of their learning. 

Syntax Learned:

•	def function_name(df): - Defines the function name and uses “df” as a parameter

•	return df[‘column_name’] – Returns the values within the specific column name

•	.nunique() – is used to count the number of unique values in a series or dataframe. It stands for ‘number of unique’ 

•	.count() – is used to count the number of non-null (non-missing) values in a series or dataframe

•	.sum() – is used to calculate the sum of values in a series or dataframe 

•	.mean() – is used to calculate the mean (average) of values in a series or dataframe. This is the sum of all values divided by how many there are.

•	.len() – used to get the length or number of items in an object 

•	.index() – is used to access the index of a pandas object, such as a series or dataframe

•	.set_index – is used to set one or more columns as the index of a dataframe

•	.shape – is used to retrieve the dimensions (shape) of the array or dataframe

•	.values - is used to retrieve the underlying NumPy array of a pandas DataFrame or Series. It returns a NumPy array representation of the data, allowing for easy integration with other NumPy or mathematical operations.

•	.append() - is used to add an element to the end of a list or another iterable object. It is a commonly used method to extend a list by appending elements. 

•	.map() - is a method available in various contexts, such as strings, lists, and pandas Series. Its purpose is to apply a specified function to each element of an iterable (like a list or Series) and return an iterable of the results.

•	.format() - is used to format strings. It provides a flexible way to embed variables and expressions inside a string, allowing you to create strings that incorporate dynamic values.

•	.sort_values() - is used to sort the values of a DataFrame or Series along a specified axis. This method is particularly useful when working with tabular data, where you might want to reorder rows based on the values in one or more columns.

•	.groupby() - is used for grouping data based on some criteria. It allows you to split a DataFrame into groups based on the values in one or more columns, and then apply a function to each group independently. 

- - -

This is submitted by Jesse Olivarez for the University of Utah: Data Analytics Bootcamp
