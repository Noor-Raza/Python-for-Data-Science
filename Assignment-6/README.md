# Python for Data Science

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
