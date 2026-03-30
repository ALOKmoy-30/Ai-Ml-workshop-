# TITANIC PREPROCESSING PROJECT

This project demonstrates a comprehensive data preprocessing workflow on the Titanic dataset. The goal is to clean, transform, and prepare the raw data for machine learning model training.

## Project Steps

1.  **Import Libraries**: Essential libraries such as pandas, numpy, sklearn's `train_test_split`, `StandardScaler`, `LabelEncoder`, and `MinMaxScaler` were imported.
2.  **Load Data**: The Titanic dataset was loaded from a CSV string into a pandas DataFrame.
3.  **Initial Data Inspection**: Displayed the first 5 rows of the dataset to get a quick overview.
4.  **Check Dataset Shape**: Printed the number of rows and columns in the dataset.
5.  **Display Column Names**: Listed all column names to understand the available features.
6.  **Check Basic Information**: Used `df.info()` to get a summary of the DataFrame, including data types and non-null counts.
7.  **Check Missing Values**: Identified the count of missing values for each column using `df.isnull().sum()`.
8.  **Drop Unnecessary Columns**: Columns like 'PassengerId', 'Name', 'Ticket', and 'Cabin' were dropped as they are not typically used for direct model training or have a high number of missing values.
9.  **Handle Missing Values**: Missing 'Age' values were imputed with the median, and 'Embarked' missing values were imputed with the mode.
10. **Separate Features and Target**: The dataset was split into input features (X) and the target variable (y, 'Survived').
11. **One-Hot Encoding**: Categorical features ('Sex', 'Embarked') were converted into numerical format using one-hot encoding.
12. **Label Encoding**: The target variable ('Survived') was label encoded.
13. **Train-Test Split**: The data was split into training and testing sets to evaluate model performance.
14. **Standardization**: Numerical features in the training and testing sets were scaled using `StandardScaler`.
15. **Normalization**: Numerical features in the training and testing sets were also scaled using `MinMaxScaler`.

## Libraries Used

*   **pandas**: For data manipulation and analysis.
*   **numpy**: For numerical operations.
*   **sklearn.model_selection.train_test_split**: For splitting data into training and testing sets.
*   **sklearn.preprocessing.StandardScaler**: For standardizing features.
*   **sklearn.preprocessing.LabelEncoder**: For encoding categorical target labels.
*   **sklearn.preprocessing.MinMaxScaler**: For normalizing features.
