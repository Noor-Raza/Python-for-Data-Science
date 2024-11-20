# Python for Data Science

# Assignment 4

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
