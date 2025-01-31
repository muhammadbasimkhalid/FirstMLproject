Investment Failure Prediction
Project Overview
This project aims to predict the likelihood of investment failure based on various features related to investor demographics, risk tolerance, investment details, and past performance. The objective is to preprocess the dataset, engineer relevant features, and build a classification model to predict whether an investment will result in failure or not.

Dataset
The dataset contains the following 18 columns:

Investor_ID: A unique alphanumeric code assigned to each investor.
Age: The investor's age in years.
Annual_Income: The investor's total income earned throughout the year.
Investment_Amount: The sum of money invested in a specific opportunity.
Risk_Tolerance_Score: A numerical representation of the investor's willingness to accept risk (higher scores indicate greater risk appetite).
Months_of_Investing_Experience: Duration of the investor's active participation in investing (in months).
Number_of_Active_Investments: The count of different investments the investor currently holds.
Potential_Return_Rate: The estimated percentage return on an investment.
Investment_Duration: The intended length of time (in months) the investment will be held.
Investment-to-Income_Ratio: The ratio of the investment amount compared to the investor's annual income.
Education: The investor's highest level of educational attainment.
Employment_Status: The investor's current employment situation (e.g., full-time, part-time, unemployed).
Marital_Status: The investor's marital status (e.g., single, married, divorced).
Owns_Property: Indicates whether the investor owns real estate (Yes/No).
Has_Dependents: Indicates whether the investor has others who financially rely on them (Yes/No).
Investment_Sector: The industry or market the investment is focused on (e.g., technology, healthcare, real estate).
Has_Investment_Advisor: Indicates whether the investor utilizes a professional investment advisor (Yes/No).
Investment_Failure: Indicates whether a past investment resulted in a loss (1 for Yes, 0 for No).
Problem Statement
The goal of this competition is to develop a classification model to predict whether an investment will fail based on the features provided. We will train the model using historical data and evaluate it using the ROC-AUC curve, which is the evaluation metric for this task.

Steps Followed
Data Preprocessing:

Handled missing values.
Categorical features encoded (e.g., Yes/No columns).
Feature scaling where necessary (e.g., using Min-Max scaling).
Feature Engineering:

Created new features such as investment-to-income ratio and risk tolerance score.
Dropped irrelevant or redundant features.
Model Selection:

Implemented multiple classification algorithms (e.g., Logistic Regression, Random Forest, XGBoost).
Tuned hyperparameters using cross-validation.
Model Evaluation:

Evaluated model performance based on ROC-AUC score.
Compared various models to select the one with the highest performance.
Technologies Used:
Python: Used for data preprocessing, model building, and evaluation.
Libraries:
Pandas & NumPy for data manipulation and preprocessing.
Scikit-learn for building and evaluating machine learning models.
Matplotlib & Seaborn for data visualization.
How to Use
Clone the repository to your local machine:

bash
Copy
Edit
git clone https://github.com/username/repository_name.git
Install the necessary dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Run the Python notebook to interact with the model:

bash
Copy
Edit
jupyter notebook
Upload new data and use the trained model to make predictions on investment failure:

Use the provided functions to load and preprocess new datasets.
The model will output predictions (1 = Failure, 0 = Success).
Evaluation Metrics
The model's performance will be evaluated using the ROC-AUC curve, which represents the trade-off between true positive rate and false positive rate.

Submission
Please ensure the following before submission:

An executed Python notebook with all steps and comments.
A transformed dataset file (with preprocessing applied).
Submit the final results to the competition organizers as per the instructions.

License
This project is licensed under the MIT License.
