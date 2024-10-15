# README.md for "Prediction of Students' Performance using Random Forest Regression"

## Project Overview
This project focuses on predicting students' academic performance using **Random Forest Regression** and **Random Forest Classification** algorithms. The dataset used in this project includes student information related to personal, family, and academic characteristics. This project was completed as part of a module on **Data Mining**.

## Features and Methods
1. **Exploratory Data Analysis (EDA)**:
   - Data cleaning and preprocessing, including handling missing values, removing duplicates, and outlier detection.
   - ![image](https://github.com/user-attachments/assets/4c112fa9-47a5-4fa6-b227-956310c33d08)

   - Merged two datasets containing information about students' performance in mathematics and Portuguese subjects.
   - **Outlier Imputation** using the **Interquartile Range (IQR)** method
   - ![image](https://github.com/user-attachments/assets/2a95d745-3113-4166-9118-50d894b6e634)

   - Analysis of the association between different variables (e.g., parental education, alcohol consumption, etc.) and students' final grades using **chi-square tests**.

2. **Factor Analysis**:
   - Performed to reduce dimensionality and identify important features.
   - ![image](https://github.com/user-attachments/assets/8f60a029-3d44-4570-a466-76137c4af6d9)

   - Six key factors were identified based on the **scree plot** and **factor loadings**.
   - ![image](https://github.com/user-attachments/assets/b79e7de4-4407-43b0-9ee2-714782a610f3)
   - ![image](https://github.com/user-attachments/assets/d9434f96-c0ab-445d-a82e-5b133ec744ac)



3. **Modeling**:
   - **Random Forest Regressor** for predicting students' final grades.
     - Achieved an **R-squared of 0.8543**, indicating that the model explains 85.43% of the variance in final grades.
     - After hyperparameter optimization, the model performance improved with an **R-squared of 0.8710**.
   - **Random Forest Classifier** for categorizing students into performance categories (Poor, Average, Good).
     - Achieved an accuracy of **92%** with minimal misclassifications.

4. **Optimization**:
   - Hyperparameters were fine-tuned using **GridSearchCV** for both regression and classification tasks to enhance model performance.
   - Key hyperparameters optimized include `n_estimators`, `max_depth`, `min_samples_split`, and `min_samples_leaf`.

## Project Structure
- `data/`: Contains the datasets used for training and testing the models.
- `notebooks/`: Jupyter notebooks with detailed step-by-step analysis and modeling.
- `scripts/`: Python scripts for data preprocessing, model training, and evaluation.
- `results/`: Model performance metrics and other results.
- `images/`: Contains all images used in the README file (e.g., pipeline diagrams).

## Pipeline Diagram
The following image represents the data pipeline used in this project, from data preprocessing to model optimization.

![image](https://github.com/user-attachments/assets/b07f42b4-928d-49ba-9cd5-3c7589e52093)


## Results
- The **Random Forest Regressor** explains over 85% of the variance in students' final grades with a mean squared error of **1.5488**.
- The **Random Forest Classifier** demonstrates strong predictive performance with an accuracy of **92%** for classifying students into different performance categories.

## Future Work
- Further optimization of the model using **ensemble techniques** like **Gradient Boosting** or **XGBoost**.
- Incorporating more features such as psychological or socio-economic factors to improve prediction accuracy.
- Deployment of the model into a real-time application for monitoring student performance over time.

## Authors
- Dirdh Patel - MSc. Artificial Intelligence (U2366489)


