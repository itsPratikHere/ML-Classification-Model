🚢 Titanic Survival Prediction: Random Forest Analysis

📌 Project Overview
This project implements a machine learning pipeline to solve the classic Titanic: Machine Learning from Disaster challenge. Using a Random Forest Classifier, the model predicts passenger survival based on demographic and socio-economic features.

The objective was to move beyond simple accuracy and understand the underlying factors—such as gender and ticket class—that determined survival during the 1912 tragedy.

🛠️ Technical Stack
Language: Python

Libraries :
Pandas & NumPy for data manipulation.
Seaborn & Matplotlib for Exploratory Data Analysis (EDA).
Scikit-Learn for model training, preprocessing, and evaluation.

🧬 Methodology & Pipeline
1. Data Preprocessing
Missing Value Imputation: Handled null values in the age and embarked columns using median and mode strategies to prevent data bias.
Feature Encoding: Converted categorical variables (Sex, Embarked) into numerical formats using mapping and One-Hot Encoding to make them compatible with Scikit-Learn.
Feature Selection: Dropped high-cardinality or redundant features (like Cabin and Name) to reduce model noise.

2. Model Architecture
I chose a Random Forest Classifier as the primary model.
Why Random Forest? It handles non-linear relationships effectively and is robust against overfitting compared to a single decision tree.
Configuration: 100 decision trees (n_estimators=100) were used to build an ensemble majority-vote system.

📊 Results
Model Performance
The final model achieved a predictive accuracy score of 81.01%.

Feature Importance
The analysis revealed that the top three predictors of survival were:

1. Sex: Validating the "Women and children first" historical protocol.

2. Fare: Indicating a strong correlation between socio-economic status and survival.

3. Age: Confirming that younger passengers were prioritized during evacuation.

🚀 How to Run
1.Clone the repository: git clone https://github.com/YOUR_USERNAME/titanic-survival-prediction.git

2.Install dependencies: pip install pandas seaborn scikit-learn matplotlib

3.Run the notebook: jupyter notebook Titanic_Survival_Prediction.ipynb
