# ML-projects-Oral-Cancer-Reccurence-Analysis-and-Visualize
project based on healthcare domain

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

----------------------------------------------------------------*******************-----------------------------------------------------------

Let's break down each part in the context of the three stages of cancer recurrence:
In the context of oral cancer data analysis, "recurrence" likely refers to whether the cancer has returned after initial treatment. Recurrence is typically classified into different categories to denote the severity or stage of the recurrence. While the specific definitions may vary depending on the dataset or medical protocol, here's a general interpretation:

Recurrence 1: This could indicate the first occurrence of cancer recurrence after the initial treatment. It may suggest that the cancer has returned but is at an early stage or is localized.

Recurrence 2: This might signify a second occurrence of cancer recurrence, indicating that the cancer has returned again after the initial treatment. It could imply a more advanced stage compared to Recurrence 1, 
              potentially involving larger tumors or spreading to nearby tissues.
              
Recurrence 3: This could represent a third occurrence of cancer recurrence, indicating a further progression of the disease. Recurrence 3 might suggest that the cancer has become more aggressive or resistant to treatment, 
              potentially involving metastasis to distant organs or multiple sites within the body.

=>It's essential to note that the exact definitions of recurrence stages can vary across medical institutions or research studies, so it's essential to refer to the specific definitions provided within the dataset or medical literature for precise interpretation.







