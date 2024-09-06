Aerospace Investment Rating Analysis
Project Overview

This project focuses on analyzing the SpaceFund Realty (SFR) rating of aerospace companies and their missions. The SFR is a rating system that ranges from 1 to 9, where a higher score indicates a more developed and stable company. The objective is to help investors make informed decisions by analyzing the companies based on factors such as launch cost, payload, mission type, and more.
Dataset

The dataset includes various features related to aerospace companies and their missions:
Column Name	Description
Company	Name of the company
SFR	SpaceFund Realty rating of the company
Payload(kg)	Payload of the mission (in kilograms)
Launch Cost (million USD)	Launch cost of the mission (in million USD)
Price per kg	Price per kg of the payload
Launch Class	Launch class of the mission (Small, Medium, Heavy, Tourism)
Orbit Altitude	Orbit altitude of the mission (LEO, GTO, Suborbital, Lunar)
Tech Type	Technology type of the mission (Rocket, Spaceplane, Balloon)
Country	Country of origin of the company
HQ Location	Headquarters location of the company
Description	Description of the company or mission
Data Preprocessing

    Handling Missing Data:
        Dropped the HQ Location column as it is redundant with the Country column.
        Filled missing values in Launch Class and Orbit Altitude with the mode.
        Dropped the Funding ($M) column due to significant missing data.

    Categorization:
        Grouped the companies based on their descriptions into 7 categories:
            Launch Vehicle Development
            Launch Services
            Balloon-Based Technologies
            Space Tourism and Suborbital
            Satellite Technology and Services
            Innovative Propulsion Technologies
            Space Access and Technology Innovation

    Handling Outliers:
        Replaced invalid zero values in columns like Payload, SFR, and Launch Cost with the mean/median.

Exploratory Data Analysis (EDA)

The EDA helped in understanding the distribution of the data and exploring relationships between the variables:

    Country-wise Analysis: The United States has the highest number of missions and companies with higher SFR ratings, followed by China and the UK.
    Mission Type: Rocket-type missions dominate the dataset, with a focus on small payloads and LEO missions.
    Launch Cost Distribution: Most missions had a launch cost between $5-10 million, with only a few exceeding $100 million.
    Payload vs SFR: There is a positive correlation between the mission payload and SFR rating, with more developed companies handling heavier payloads.

Data Visualizations

The key visualizations created include:

    Number of Missions per Country
    Mission Type Distribution
    Launch Class vs SFR
    Payload vs SFR
    Orbit Altitude vs SFR

Machine Learning Models

Two machine learning models were used to predict the SFR rating:

    Random Forest Classifier
        Hyperparameter tuning using GridSearchCV.
    Decision Tree Classifier
        Hyperparameter tuning for better model comparison.

Model Evaluation

The models were evaluated using:

    Confusion Matrix
    Classification Report
    Accuracy and F1-score

Conclusion

    US-based aerospace companies dominate the dataset, with a higher number of companies showing a strong SFR rating (>6).
    Rocket-type missions focusing on small payloads to LEO are common among less-developed companies with low SFR ratings (2-3).
    Larger payloads and complex missions are more frequent among companies with higher SFR ratings, indicating better stability and development.

Technologies Used

    Python: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn
    Jupyter Notebook: For data exploration and model development
    Machine Learning: Random Forest Classifier, Decision Tree Classifier
    GridSearchCV: For hyperparameter tuning

Future Enhancements

    Incorporate additional datasets for further refinement of SFR predictions.
    Explore other models such as Support Vector Machines (SVM) or Gradient Boosting.
    Develop a dashboard for real-time data analysis and visualization.
