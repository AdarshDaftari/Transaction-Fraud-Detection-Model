How the Project Works
1. Business Problem Framing

The project simulates a real-world scenario where a company, “Blocker Fraud,” specializes in detecting fraudulent mobile transactions. Its business model is highly performance-driven:

Earns 25% of the transaction value when a fraud is correctly detected.

Earns 5% when a transaction is incorrectly marked as fraud (a false positive).

Must fully reimburse the customer when real fraud is missed (false negative), thus creating high stakes for model accuracy.

Data Pipeline and Preparation

The project follows a structured data science workflow:

Step 1: Data Collection & Initial Exploration
Load transaction data, handle missing values, compute descriptive statistics like skewness, kurtosis, mean, median, etc., to understand data characteristics. 
GitHub

Step 2: Feature Engineering
Develop feature hypotheses (e.g., transaction frequency, amounts, patterns), possibly visualized through a mind map, to derive features that could help distinguish between fraud and legitimate transactions. 
GitHub

Step 3: Data Filtering
Remove irrelevant columns, such as customer IDs, hash codes, or invalid age entries, ensuring cleaner and business-relevant data. 
GitHub

Step 4: Exploratory Data Analysis (EDA)
Perform univariate, bivariate, and multivariate analyses to test the formulated hypotheses and understand relationships in the data. 
GitHub

Step 5: Data Preparation
Apply encoding, rescaling, and techniques to handle class imbalance (such as oversampling/subsampling) to optimize model learning. 
GitHub

Step 6: Feature Selection
Use feature selection algorithms like Boruta to identify the most informative variables, reduce dimensionality, and lower the risk of overfitting. 
GitHub

3. Modeling & Evaluation

The model development follows a multi-step approach:

Step 7: Training Multiple Models
Several machine learning algorithms are implemented and compared, including:

Logistic Regression

K-Nearest Neighbors (KNN)

Support Vector Machine (SVM)

Random Forest

XGBoost

LightGBM

A Neural Network model 
GitHub

Step 8: Hyperparameter Tuning
For the best-performing model, tuning is applied to improve accuracy, precision, recall, and overall F1 score. 
GitHub

Step 9: Model Validation and Business-Relevant Metrics
After training and validation, the model is evaluated on unseen data to assess:

Balanced Accuracy

Precision

Recall

F1 Score

Financial Impact Metrics—including expected company revenue, losses from false positives, reimbursements for false negatives, and overall profit. 
GitHub

Step 10: Deployment Strategy
Final step includes preparing the model for deployment, likely via a Flask API, enabling integration into real-world systems. 
GitHub

Highlights & Business Value

Structured, End-to-End Pipeline: Covers all stages—from data ingestion to business-aligned deployment.

Strong Focus on Business Metrics: Goes beyond model accuracy to evaluate financial risk and revenue impact.

Feature Optimization: Uses Boruta to ensure only meaningful variables enter the model, enhancing robustness.

Model Comparison: Evaluates a wide spectrum of algorithms to identify the best fit.

Deployment-Ready: Integrates API deployment planning for real-world usability.
