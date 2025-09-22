# Elevate Labs - AI & ML Internship Task 1

### Objective
This project is part of the Elevate Labs AI & ML Internship, where the primary goal was to learn and apply fundamental data cleaning and preprocessing techniques on a raw dataset.

### Tools Used
* **Python**: The core programming language for the task.
* **Pandas**: Used for data manipulation and analysis, including handling missing values.
* **NumPy**: A library for numerical operations.
* **Matplotlib/Seaborn**: Used for data visualization, specifically for detecting and visualizing outliers.
* **scikit-learn**: Used for feature scaling and encoding.

### Steps Performed
1.  **Data Loading & Initial Exploration**: The Titanic dataset was loaded, and basic information like data types and the presence of missing values was checked using `df.info()` and `df.isnull().sum()`.
2.  **Handling Missing Values**:
    * Missing values in the **'Age'** column were filled with the median to avoid bias from outliers.
    * Missing values in the **'Embarked'** column were filled with the most frequent value (mode).
    * The **'Cabin'** column was dropped due to a high number of missing values.
3.  **Categorical Feature Encoding**:
    * The **'Sex'** column was converted into numerical values using Label Encoding.
    * The **'Embarked'** column was converted into numerical columns using One-Hot Encoding.
4.  **Outlier Detection and Removal**: Outliers in the **'Fare'** column were visualized using a boxplot and then removed using the Interquartile Range (IQR) method to ensure a clean dataset.
5.  **Feature Scaling**: Numerical features like 'Age' and 'Fare' were standardized using `StandardScaler` to prepare the data for machine learning models.

This project successfully demonstrates the entire data preprocessing pipeline, from handling missing data and encoding categorical features to managing outliers and scaling numerical data.
