# ML-projects-Oral-Cancer-Reccurence-Analysis-and-Visualize
Disclaimer: we can't upload Dataset here because it is confedential, we are working with Ramaiah Memorial Hospital Dataset.

project based on healthcare domain

------------------------------------------------------------------------------------------------------------------------------------
Objective: This program effectively loads a cancer recurrence dataset, preprocesses the data, and uses a Random Forest classifier to predict cancer recurrence. The model is tuned using GridSearchCV to find the best parameters. Various visualizations provide insights into the data and model performance, making it easier to interpret the results. The use of feature scaling, hyperparameter tuning, and comprehensive evaluation ensures the model is well-optimized and provides accurate predictions.
------------------------------------------------------------------------------------------------------------------------------------
This code performs various tasks related to analyzing oral cancer recurrence data and building predictive models.

Data Loading and Preprocessing:
The code imports necessary libraries and loads the oral cancer dataset from an Excel file (Dataset_OSCC (2) (1) (1).xlsx).
It encodes the categorical target variable 'Recurrence' into numerical format using a label encoder.
Categorical columns in the dataset are identified and converted to numerical format.

Data Visualization:
It creates visualizations to understand the data, including a scatter plot matrix, correlation heatmap, distribution of cancer recurrence, and box plots of key features.

Data Splitting:
The dataset is split into training and testing sets with an 80-20 ratio.

Model Building and Hyperparameter Tuning:
Three classifiers (GradientBoosting, RandomForest, AdaBoost) are defined.
Hyperparameter tuning is performed for each classifier using Randomized Search Cross-Validation to find the best models.

Model Evaluation:
The best models for each classifier are evaluated using accuracy scores, classification reports, and confusion matrices.
Analysis of Recurrence and Mortality Factors:

Factors related to cancer recurrence (e.g., age, sex, cancer stage) are analyzed using box plots.
Additional visualizations are provided based on cancer stages if 'Pathologic group Stage' data is available in the dataset.
The code provides a comprehensive analysis of oral cancer recurrence data, including data preprocessing, visualization, model building, evaluation, and interpretation of results, considering three stages of cancer recurrence.
--------------------------------------------------------------------------------------------------------------------------------------

Let's break down each part in the context of the three stages of cancer recurrence:
In the context of oral cancer data analysis, "recurrence" likely refers to whether the cancer has returned after initial treatment. Recurrence is typically classified into different categories to denote the severity or stage of the recurrence. While the specific definitions may vary depending on the dataset or medical protocol, here's a general interpretation:

Recurrence 0: This could indicate the first occurrence of cancer recurrence after the initial treatment. It may suggest that the cancer has returned but is at an early stage or is localized.

Recurrence 1: This might signify a second occurrence of cancer recurrence, indicating that the cancer has returned again after the initial treatment. It could imply a more advanced stage compared to Recurrence 1, 
              potentially involving larger tumors or spreading to nearby tissues.
              
Recurrence 2: This could represent a third occurrence of cancer recurrence, indicating a further progression of the disease. Recurrence 3 might suggest that the cancer has become more aggressive or resistant to treatment, 
              potentially involving metastasis to distant organs or multiple sites within the body.

=>It's essential to note that the exact definitions of recurrence stages can vary across medical institutions or research studies, so it's essential to refer to the specific definitions provided within the dataset or medical literature for precise interpretation.
---------------------------------------------------------------------------------------------------------------------------------------
Explaination file::  oral_caner_(1) (1) (1).ipynb

This bar chart shows the relationship between Clinical Tumor size (cT) and Clinical Node involvement (cN) in terms of their counts.

Tumor Sizes (cT)
T1: The tumor is small, no bigger than(2 cm or less).
T2: The tumor is bigger than a (more than 2 cm but 4 cm or less).
T3: The tumor is bigger than a (more than 4 cm).
Advanced Tumor Sizes
T4: The tumor has grown into nearby areas and can be split into:
T4a: The tumor has spread into nearby structures like bones, deep muscles of the tongue, the maxillary sinus, or the skin of the face. This is more advanced .
T4b: The tumor has spread even further into more critical areas like the spaces around the jaw muscles, the skull base, or it has wrapped around the internal carotid artery. This is very advanced and extensive.

Clinical Node Involvement (cN)
N0: No spread to nearby lymph nodes. Think of it as no weeds spreading to other parts of the body.
N1 to N3 - Increasing Spread:
N1: The cancer has spread to one nearby lymph node, and it's small (3 cm or less).
N2 - More Spread, but Still Manageable:
N2: The cancer has spread more than N1, and it can be:
N2a: One larger nearby lymph node, bigger than 3cm but no larger than 6cm or less. 
N2b: Several nearby lymph nodes affected, but none are bigger than 6cm.
N2c: Cancer has spread to lymph nodes on both sides or the opposite side of the body, but all are still no larger than a 6 cm.
N3 - Extensive Spread:
N3: The cancer has spread to one or more lymph nodes and at least one is larger than a more than 6 cm.

Key Points:
X-axis (Horizontal): Represents the Clinical Tumor size (cT) which ranges from 0 to 4.
Y-axis (Vertical): Represents the count (number of cases) for each combination of cT and cN.
Colors: Represent different levels of Clinical Node involvement (cN) from 0 to 6.

Summary:
The chart shows that smaller tumor sizes (0, 1, and 2) have higher counts and more variation in node involvement, while tumor sizes (3 and 4) have fewer cases but still show some node involvement. And larger tumor size (5 & 6) have very few cases still have some less variation in node involvement.                                   









