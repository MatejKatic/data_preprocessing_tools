Data Preprocessing Tools

The project reads a CSV dataset and performs the following preprocessing steps:

    Missing Data Handling: Replaces missing values in selected numerical features with the mean value using scikit-learn’s SimpleImputer.
    Categorical Data Encoding: Transforms categorical data using one-hot encoding for independent variables and label encoding for the dependent variable.
    Dataset Splitting: Divides the dataset into training and test sets to facilitate model evaluation.
    Feature Scaling: Standardizes numerical features to improve the performance of many machine learning algorithms.

Project Structure

    Data.csv: The input dataset.
    data_preprocessing_tools.py: The main Python script containing the preprocessing pipeline.
    data_preprocessing_tools.ipynb: A Jupyter Notebook version of the preprocessing pipeline for interactive use.

Requirements:

Make sure you have Python 3.x installed along with the following packages:

    NumPy
    Pandas
    Matplotlib
    scikit-learn

You can install the required packages using pip:

pip install numpy pandas matplotlib scikit-learn

Usage

To run the preprocessing script, simply execute:

python data_preprocessing_tools.py

This will:

    Load the dataset from Data.csv.
    Handle missing values in specified columns.
    Encode categorical features appropriately.
    Split the data into training and test sets.
    Apply feature scaling to standardize the data.

The processed data is printed to the console, allowing you to review the intermediate outputs at each step.
Preprocessing Steps Detailed

    Import Libraries and Load Data:
        The script imports necessary libraries and reads the CSV file into a Pandas DataFrame.
    Handling Missing Data:
        Utilizes SimpleImputer to replace missing values with the mean of the column.
    Encoding Categorical Data:
        Applies one-hot encoding on the independent variable(s) using ColumnTransformer and OneHotEncoder.
        Uses LabelEncoder to encode the dependent variable.
    Splitting the Dataset:
        Uses train_test_split to create training and test subsets, ensuring that the model evaluation is fair.
    Feature Scaling:
        Standardizes the features using StandardScaler to ensure that all numerical variables are on a similar scale.
