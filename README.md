# Python for Data Science

# Assignment-1
**Description:**
Assignment 1 branch contains solutions to basic Python exercises, covering topics such as arithmetic operations, string manipulation, lists, dictionaries, tuples, sets, control flow, and functions.

## List of Exercises:

### 1. Syntax and variables
    Exercise 1: Print a Greeting
    A simple Python program to print a greeting message, such as "Hello, Python!".
    Exercise 2: Basic Arithmetic
    A Python program that defines two variables `a` and `b`, then prints their sum, difference, product, and quotient.
    Exercise 3: String Manipulation
    A Python program that defines a variable `name` and prints "Hello, [name]!" where `[name]` is the value of the variable.

### 2. Lists and Dictionaries
    Exercise 4: Lists
    A program that creates a list of five universities and prints the entire list, along with the first and last university in the list.
    Exercise 5: Dictionaries
    A program that creates a dictionary called `student` with keys: `name`, `age`, and `grade`. It prints each key-value pair in the dictionary.

### 3. Tuples and Sets
    Exercise 6: Tuples
    A program that defines a tuple `coordinates` with two values representing a point in 2D space and prints the values.
    Exercise 7: Sets
    A program that creates a set of colors, adds a new color, tries adding a duplicate color, and merges with another set.

### 4. Control flow
    Exercise 8: Conditional Statements
    A program that takes an input number from the user and checks whether it is positive, negative, or zero.
    Exercise 9: For Loop
    A program that iterates through a list of numbers from 1 to 5 and prints each number.
    Exercise 10: While Loop
    A program that uses a `while` loop to print numbers from 1 to 5.
    Exercise 11: Match Statement (Python 3.10+)
    A program that asks the user for a grade and uses the `match` statement to print a corresponding message.

### 5. Function
    Exercise 12: Define a Function
    A function `greet` that takes a name as an argument and prints "Hello, [name]!".
    Exercise 13: Function with Return Value
    A function `square` that takes a number as an argument and returns its square.
    Exercise 14: Function with Default Parameters
    A function `multiply` that takes two parameters, `a` and `b`, and returns their product. The second parameter has a default value of 1.

### 6. Combining all we learned
    Exercise 15: List Comprehension
    A program that uses list comprehension to generate a list of squares of numbers from 1 to 10.
    Exercise 16: Nested Data Structures
    A program that creates a dictionary of students and their grades, then calculates the average grade for each student.
    Exercise 17: Simple Calculator
    A calculator program that performs basic operations (+, -, *, /) based on user input.

# Assignment-2

**Description:**
Assignment branch contains a set of basic Python exercises aimed at practicing fundamental programming concepts such as conditionals, loops, list comprehension, and functions.
The exercises are designed to be easy to follow, with explanations and examples provided for each.

## List of Exercises:

### Exercise 1: FizzBuzz Function
    
    FizzBuzz is a classic programming problem. The function takes a number n and prints all numbers from 1 to n.
    However, for multiples of 3, it prints "Fizz", for multiples of 5, it prints "Buzz", and for multiples of both 3 and 5, it prints "FizzBuzz".
    For all other numbers, it simply prints the number itself.

### Exercise 2: Basic Data Filtering
    
    In this exercise, a list containing mixed data types (integers, strings, and floats) is created.
    The task is to filter the list and create a new list that contains only integers using list comprehension.
    This exercise helps practice list manipulation and filtering based on data types.
    
### Exercise 3: Simple To-Do List
    
    This exercise simulates a basic to-do list application.
    The program starts with an empty list, and two functions are defined:
        - add_task(task): Adds a task to the to-do list.
        - show_tasks(): Displays all tasks currently in the list.
    Users can call add_task() to add new tasks and show_tasks() to print the entire list of tasks.

### Exercise 4: Temperature Converter
    
    This exercise involves converting temperatures from Celsius to Fahrenheit using a function.
    The function celsius_to_fahrenheit(celsius) applies the conversion formula and prints the results for a list of temperatures in Celsius.
    
# Assignment-3

This assignment implements a simple Course Registration System using Python. The system consists of three main classes: **Course**, **Student**, and **Registration**.

### Features
- **Course Class**: Represents a course with a name, description, and methods to manage enrolled students.
  - Add and remove students from the course.
  - Display all students enrolled in the course.

- **Student Class**: Represents a student with a name, ID number, address, and a list of enrolled courses.
  - Enroll in and drop courses.
  - Assign grades for each course and calculate the Grade Point Average (GPA).
  - Display all registered courses and their grades.

- **Registration Class**: Manages the overall registration process, including a list of students and courses.
  - Enroll students in courses and drop courses.
  - Display all available courses and registered students.

### Exercises Overview

1. **Course Class**: Implement a class to manage course details and student enrollments.
2. **Student Class**: Create a class to manage student information, course enrollments, and grades.
3. **Registration Class**: Develop a central management class that oversees both courses and students.
4. **GPA Calculation**: Enhance the Student class to include grade assignments and a method to calculate GPA based on enrolled courses.

### Usage
The system allows you to create instances of students and courses, manage enrollments, and calculate GPAs. Example usage is provided to demonstrate the functionalities of the classes.

# Assignment 4

## Basic Libraries I

### Overview: Satellite Annotations Analysis
This assignment processes a collection of satellite annotation files, analyzing and organizing the data based on specific criteria such as date, satellite number, and unique region. The file naming convention includes metadata like date, time, satellite number, and region, which we leverage to extract insights.

### Exercises

Given a zip file with a subfolder with multiple annotations, where the name convention for each one of them is: 

{DATE}_{TIME}_SN{SATELLITE_NUMBER}_QUICKVIEW_VISUAL_{VERSION}_{UNIQUE_REGION}.txt

where:

- DATE expressed as YYYYMMDD (year, month and day), e.g. 20241201, 20230321 ...
- TIME expressed as HHMMSS (hour, minutes and seconds), e.g. 2134307
- SATELLITE_NUMBER an integer that represents the satellite number.
- VERSION provides the version of the pipeline, e.g. "0_1_2", "1_3_1" ...
- UNIQUE_REGION provides a unique location in the form of a string, e.g SATL-2KM-10N_552_4164

Find out the following thing about your data:

1. How many files the annotations folder has.
2. How many of them follow the name convention expressed above.
3. How many of annotations you have per month and year. Which month has more annotation files.
4. Create a new annotations folder with multiple folders corresponding to a month.
5. Print all the annotations from the most recent to the oldest one. 
6. How many different satellites there are, how many annotations we have per satellite number, and which one was used in the most recent annotation file. 
7. How many unique regions there are.

some tips:
- str class has a method called split, you can use it to get each field per annotation.
- you can use sort from numpy on strings.

# Assignment 5

## Basic Libraries II

## Overview
This project processes annotation files stored in a directory and performs various operations such as counting annotations, grouping them by month, saving the data in different formats, and organizing it for easier analysis. The exercises showcase how to work with file handling, datetime manipulation, and data serialization using JSON and Pickle.

## Exercises

### 1. Count Annotations Per Month and Year
- **Description**: Counts the number of annotation files for each month and year based on the dates in their filenames. Identifies the month with the highest number of annotations and displays the data as a sorted table.

### 2a. Save Data in JSON Format
- **Description**: Groups annotations by month into a dictionary where:
  - Each **key** is a month (e.g., `2024-06`).
  - Each **value** is a list of annotation filenames for that month.
  The data is saved in JSON format, and the JSON file is reloaded to verify correctness.

### 2b. Save Data in Pickle Format
- **Description**: Saves the same grouped dictionary as in 2a but using Pickle, a binary format. The Pickle file is reloaded and displayed in a tabular format to ensure its integrity.

### 2c. Enhance Data with Names and Dates
- **Description**: Modifies the grouped dictionary so that each entry for a month contains:
  - A list of dictionaries, where each dictionary has:
    - `name`: The annotation filename.
    - `date`: The date (as a `datetime` object) extracted from the filename.
  This detailed structure is saved in JSON format for easier future use.

### 3. Sort Annotations from the Second Half of 2024
- **Description**: Extracts annotations from the second half of 2024 (June to December) and sorts them chronologically. The output is displayed as a list, showing both filenames and dates in ascending order.

# Assignment 6

## Pandas I

## Overview

This notebook includes exercises to analyze two datasets: **Netflix** and **Titanic**. Below are the exercises and their descriptions.

## Netflix Dataset Exercises

1. **Is there any missing rating?**
   - **Description:** Counting the number of missing values in each column to understand data completeness.

2. **How many films in 2021 correspond to your country?**
   - **Description:** Replacing missing values in the 'country' column with "Unknown" to handle incomplete data.

3. **What's the number of movies in 2020 with full information?**
   - **Description:** Filtering the dataset to keep only entries of type "TV Show."

4. **Give me the year with more titles.**
   - **Description:** Calculating the number of entries for each unique value in the 'rating' column to understand content distribution.

5. **And what has been the average in terms of releases from 2010.**
   - **Description:** Adding a new column, **content_age**, to calculate the age of the content by subtracting its release year from the current year.

## Titanic Dataset Exercises

1. **Calculate Gender-Based Survival Percentage**
   - **Description:** Calculating the survival percentage for each gender by dividing the number of survivors by the total passengers for each gender.

2. **Calculate Survival Percentage Grouped by Gender and Class**
   - **Description:** Calculating survival percentages for each combination of gender and passenger class.

# Assignment 7

## Pandas II

## Overview  
This assignment focuses on performing various DataFrame manipulations using Python's **pandas** library. It includes tasks like creating new columns, merging DataFrames, and extracting specific information from text columns. These exercises are designed to improve your data preprocessing and transformation skills.

## Exercises

### Exercise 1: Creating Professor Initials
**Description:** We need to extract the initials of each professor's first and last names and store them in a new column called professor_initials.


### Exercise 2: Given the dataframe below. Use **join** to combine this new DataFrame with the original one based on the professor column.
**Description:** We will merge the original DataFrame and the new df_courses DataFrame using the professor column as the key.

### Exercise 3: Combine the original df and df_courses DataFrames.
**Description:** We combine two DataFrames (df and df_courses) based on the common column professor to include the course information for each professor.

### Exercise 4: In the professor column, create a new column professor_last_name by extracting the last name of each professor using string operations.
**Description:** We extract the last name of each professor from the professor column using string operations and store it in a new column called professor_last_name.

# Assignment 8

## Plotting

## Overview
In this assignment, we are using Python's Seaborn library to visualize and analyze a dataset containing information about students, including their study time, grades, courses, gender, and more. Each exercise involves creating a specific type of plot to gain insights from the data.

## Exercises

### Exercise 1: Create a lineplot showing how Study Time varies by Student Name. Which student has the highest study time?
**Description:** We are plotting a line to show how much time each student spends studying.

### Exercise 2: Plot a histogram (histplot) of Grade and determine which grade range has the highest frequency of students.
**Description:** We are creating a bar chart to see how many students fall into each grade range.

### Exercise 3: Create an ECDF plot (ecdfplot) for Grade. What is the percentage of students scoring less than 85?
**Description:** We are plotting cumulative percentages of grades and calculating the percentage of students with grades below 85.

### Exercise 4: Create a stripplot showing Grade distribution for each Course. Which course has the most spread in grades?
**Description:** We are plotting individual grades for each course to see their spread.

### Exercise 5: Create a swarmplot to show the relationship between Gender and Study Time. Which gender has a higher average study time?
**Description:** We are showing the distribution of study times for males and females.

### Exercise 6: Plot a pointplot to show the average Grade for each Course. Which course has the highest average grade?
**Description:** We are plotting the average grade for each course to compare performance.

---
