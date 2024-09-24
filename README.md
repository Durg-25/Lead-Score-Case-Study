# Lead Scoring Case Study

## Objective
X Education, an online education company, wants to improve its lead conversion rate. They acquire leads through various sources such as website forms, referrals, and marketing efforts. Currently, their lead conversion rate is approximately 30%. The goal of this project is to build a logistic regression model that assigns a lead score (between 0 and 100) to each lead, indicating how likely a lead is to convert. This will help the company focus its sales efforts on high-potential leads, or "hot leads," to improve overall efficiency and conversion rates.

## Steps Followed

### 1. **Reading Data**
   - Import the dataset containing information about leads.
   - Load the dataset using pandas for analysis.

### 2. **Cleaning Data**
   - Remove duplicates and handle missing values.
   - Standardize text fields and clean outliers.
   - Check and remove unnecessary columns that are not relevant for analysis.

### 3. **Exploratory Data Analysis (EDA)**
   - Analyze the key patterns and trends in the dataset.
   - Plot and visualize data distributions, correlations, and relationships between features and target variable (`Converted`).
   - Identify key features that impact lead conversion.

### 4. **Creating Dummy Variables**
   - Convert categorical variables into dummy/indicator variables using `pd.get_dummies()`.

### 5. **Splitting Data**
   - Split the dataset into training and test sets using `train_test_split()` for model building and validation.
   - Typical split ratio: 70% for training and 30% for testing.

### 6. **Building the Logistic Regression Model**
   - Build a logistic regression model using `sklearn`’s `LogisticRegression`.
   - Fit the model to the training data.
   - Optimize the model using techniques such as feature selection, regularization, or handling multicollinearity (e.g., using VIF).

### 7. **Making Predictions**
   - Use the trained logistic regression model to predict the probability of conversion for the leads in the test dataset.
   - Convert probabilities into lead scores ranging from 0 to 100.

### 8. **Model Evaluation**
   - Evaluate the model's performance using metrics such as accuracy, precision, recall, and F1-score.
   - Generate the confusion matrix to understand false positives and false negatives.

### 9. **ROC Curve**
   - Plot the ROC Curve to assess the model's performance in distinguishing between classes.
   - Calculate the Area Under the Curve (AUC) to evaluate the model's discriminative ability.

### 10. **Prediction on Test Set**
   - Test the model on the unseen test dataset to verify its performance.
   - Assign lead scores and make final predictions on the test dataset.

### 11. **Precision-Recall**
   - Analyze the precision-recall tradeoff to optimize for better lead classification.
   - Calculate Precision, Recall, and F1 score to evaluate model performance for potential lead identification.


