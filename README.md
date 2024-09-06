Aerospace Investment Rating Analysis
Project Overview

The Aerospace Investment Rating Analysis project aims to assist investors in making informed decisions by analyzing the SpaceFund Realty (SFR) ratings of aerospace companies. These ratings are based on factors such as missions, payloads, and launch costs. The SFR rating ranges from 1 to 9, with higher ratings indicating more established and stable companies.
Objectives:

    Group aerospace companies based on key characteristics such as their description, mission type, payload, and launch cost.
    Perform exploratory data analysis (EDA) to uncover relationships between the SFR rating and independent variables.
    Build and evaluate machine learning models to predict the SFR ratings of aerospace companies.

Data Preprocessing
1. Grouping by Company Description:

Categorized the unique values in the description column into seven major categories for easier analysis.
2. Outlier Removal:

Identified and removed outliers to ensure that models were trained on accurate data and not skewed by extreme values.
3. Label Encoding:

Converted categorical columns such as company descriptions, mission types, and orbit classes into numerical values using label encoding for machine learning compatibility.
4. Missing Data Handling:

Handled missing values by either imputing them with appropriate statistical measures (e.g., mean, median) or removing records where necessary.
Exploratory Data Analysis (EDA)

The following analyses were performed to gain insights into the dataset:

    Distribution Plots for variables such as launch cost, payload, and SFR to observe their spread.
    Bar Charts to visualize the number of companies from each country and their corresponding SFR ratings.
    Box Plots to investigate the relationships between launch cost, payload, and SFR, with a focus on identifying outliers.
    Correlation Matrix Heatmap to explore relationships between the independent variables and the SFR rating.

Model Building

The following machine learning models were used to predict the SFR ratings:

    Random Forest Classifier
    Decision Tree Classifier

Train-Test Split:

The dataset was split into 80% training and 20% testing subsets for model training and evaluation.
Model Evaluation:

    Confusion Matrix: Visualized the true vs predicted classes.
    Distribution Plot: Displayed how well the predicted SFR ratings aligned with the actual ratings.
    Classification Report: Provided accuracy, precision, recall, and F1 score to evaluate model performance.

Both models achieved 87% accuracy. However, due to the small dataset size, recall scores for predicting SFR ratings greater than 6 were lower, suggesting the need for more data to improve model performance in this range.
Conclusion

    Most aerospace companies with high SFR ratings (greater than 6) were from the US, followed by China, despite China having fewer companies.
    Higher launch costs and payloads were associated with higher SFR ratings, indicating that more established companies have the capacity for larger, more costly missions.
    Both the Random Forest and Decision Tree models performed well but could benefit from a larger dataset for predicting higher SFR ratings.

Future Improvements

    Increase the dataset: A larger dataset could improve the machine learning models' ability to predict higher SFR ratings.
    Enhance models: Consider more sophisticated models or parameter tuning to improve accuracy.

