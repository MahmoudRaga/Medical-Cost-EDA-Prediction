# Predicting Medical Costs using Machine Learning

## Description of the Project
This project focuses on analyzing a dataset containing medical cost information to uncover meaningful insights and predict healthcare charges. The primary objectives include:
1. Conducting exploratory data analysis (EDA) to understand the dataset's structure, distribution, and relationships.
2. Building regression models to predict medical costs as continuous values.
3. Transforming the problem into a classification task to label medical costs as "cheap" or "expensive" based on a defined threshold.
4. Evaluating the performance of various models to identify the best-performing approach.

## Details About the Used Approach
1. **Exploratory Data Analysis (EDA):**
   - Identified key statistical properties of the dataset (mean, median, outliers).
   - Explored relationships between features (e.g., age, BMI, smoking status) and medical charges.
   - Visualized distributions and detected outliers using boxplots.

2. **Regression Models:**
   - Used multiple models: Linear Regression, Random Forest, Gradient Boosting, and Neural Network.
   - Compared the models' performance using R², Mean Absolute Error (MAE), Mean Squared Error (MSE), and Root Mean Squared Error (RMSE).

3. **Classification Models:**
   - Converted the continuous target variable (`charges`) into binary labels:
     - "Cheap" (0): Charges below a defined threshold.
     - "Expensive" (1): Charges above the threshold.
   - Evaluated performance using precision, recall, F1-score, and accuracy.

4. **Data Preprocessing:**
   - Encoded categorical variables using one-hot encoding.
   - Standardized numerical variables for use in Neural Networks.
   - Handled outliers to improve model stability.

## Solution Architecture
1. **Data Preprocessing:**
   - **Input:** Dataset with features like age, sex, BMI, children, smoking status, region, and charges.
   - **Processing Steps:**
     - Remove outliers using IQR.
     - Encode categorical variables and scale numerical features.
   - **Output:** Preprocessed data ready for model training.

2. **Model Training:**
   - **Regression Pipeline:** Linear Regression, Random Forest, Gradient Boosting, and Neural Network.
   - **Classification Pipeline:** Logistic Regression, Random Forest, and other classifiers.

3. **Evaluation:**
   - Models were evaluated using both regression and classification metrics.
