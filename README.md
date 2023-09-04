# Data Imputation Program (Version 3.3)

This is a Python program designed for imputing missing values in a dataset using various machine learning methods. It operates on Excel files and employs multivariate imputation techniques.

## Prerequisites

Make sure you have the following libraries installed:

- pandas
- seaborn
- matplotlib
- scikit-learn

You can install these libraries using pip.

## Usage

1. Place the dataset file (e.g., "AMR-and-NSH-Buoy-Data1394-Clean-Data.xls") in the "clean-xls-files" directory.
2. Update the dataset filename in the code if necessary.

3. Run the program by executing the `main.py` script.

4. The program will load the dataset, perform data imputation using machine learning methods, and save the results in the "multivariate-method-results" directory.

## Details

- The program uses various machine learning models for imputation, such as Linear Regression, LassoCV, and Extra Trees Regressor.
- It also includes MinMax scaling to normalize the data.
- Date and time columns ("DateTime Processor" and "SunDateTime") are processed and filled with synthetic values.
- Missing values are imputed using the IterativeImputer class from scikit-learn.

## Output

The imputed dataset will be saved in CSV format in the "multivariate-method-results" directory with a filename like "AMR-and-NSH-Buoy-Data1394-normalized-mice-extra-trees-regressor.csv" depending on the method used.

## Author

ehsanasgharzde
