Insurance Dataset Analysis
Author: Hasan A. H. Srour

Student Number: 1320224116

Project Overview
This project involves loading, preprocessing, and performing Exploratory Data Analysis (EDA) on a medical insurance cost dataset (insurance.csv). The analysis is documented in a Jupyter Notebook and focuses on preparing the data for further modeling by cleaning it and visualizing key correlations and distributions.

Dataset Details
The dataset contains 1,338 initial entries and 7 columns detailing personal attributes and billed medical charges.

Columns: age, sex, bmi, children, smoker, region, charges

Data Types: 2 Float (float64), 2 Integer (int64), 3 Object/Categorical (object)

Memory Usage: ~73.3 KB

Dependencies
Ensure the following Python libraries are installed to run the notebook successfully:

pandas (Data manipulation and analysis)

numpy (Numerical operations)

matplotlib.pyplot (Data visualization)

seaborn (Statistical data visualization)

Workflow Steps
Step 1: Loading the Data
The project connects to Google Drive to access the insurance.csv file.

The data is loaded into a Pandas DataFrame.

Basic structural checks are performed using .head(), .tail(), and .info() to understand the dataset's shape and data types.

Step 2: Data Preprocessing
Missing Values: The dataset is checked using .isnull().sum(). It contains exactly 0 missing values.

Duplicates: The dataset is checked for identical rows using .duplicated().sum(). Exactly 1 duplicate row was identified and successfully removed in-place to ensure data integrity.

Step 3: Exploratory Data Analysis (EDA)
Outlier Detection: A boxplot is generated using Seaborn to visualize the distribution of the features and identify any potential outliers.

Correlation Heatmap: A 10x6 correlation heatmap is plotted specifically for the numeric columns to identify relationships between variables. The heatmap includes numerical annotations and utilizes the coolwarm color map for clear visual distinction.
