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
