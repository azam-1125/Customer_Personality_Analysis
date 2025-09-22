# Data Analyst Internship: Task 1 - Data Cleaning and Preprocessing

## Objective
The main objective of this task was to perform data cleaning and preprocessing on a raw dataset to prepare it for analysis. The dataset used is "Customer Personality Analysis."

## Tools
* **Python**: Used for writing the data cleaning script.
* **Pandas**: A powerful Python library for data manipulation and analysis.

## Key Deliverables
* A **clean and structured dataset** ready for further analysis.
* A **short summary** of the changes and cleaning process.

## Summary of the Data Cleaning Process
The following steps were taken to clean and preprocess the raw dataset:

1.  **Loaded the Dataset**: The raw `Customer Personality Analysis.csv` file was loaded into a pandas DataFrame using a tab as the delimiter, as the data was not comma-separated.

2.  **Handled Missing Values**: The `Income` column was found to have missing values. These null values were identified and filled with the mean income of the column to preserve data integrity.

3.  **Removed Duplicate Records**: No Duplicate rows were found.

4.  **Standardized Categorical Data**:
    * The `Marital_Status` column was standardized by replacing data entry errors like 'YOLO' with 'Absurd'.
    * the 'Dt_Customer' column is converted to a consistent datetime format

5.  **Created a New Feature**: A new column named 'Age' was created by subtracting the cleaned birth years from the current year to make age-related analysis possible.

6.  **Renamed Columns**:
    * All column headers were renamed to a clean, lowercase format using underscores instead of spaces (e.g., `Marital_Status` became `marital_status`).
    * 'dt_customer' column was renamed to 'date_customer' to be more descriptive

The final, cleaned dataset is available as `Customer_Personality_Analysis_Cleaned.csv`.
