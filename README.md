# **Loan Approval Prediction Project** 🏦💰

## **Meet the Team** 👓
This project was brought to life by an incredible team of three: Joel, Calvin, and Lemgo. Each team member contributed their unique expertise to tackle the challenges of loan approval prediction.

---

## **Project Overview** 📑
The primary aim of this project is to develop a machine learning model capable of predicting whether a loan application will be approved or rejected. By analyzing various applicant features, the model empowers lending institutions to make data-driven, informed decisions, thereby reducing risks and optimizing loan disbursement strategies.

---

## **About the Dataset**
The loan approval dataset serves as the cornerstone of our analysis. It is a compilation of financial records and demographic data that determine loan eligibility. Key attributes include:
- **CIBIL score**: A reflection of creditworthiness.
- **Income**: An applicant's earning capacity.
- **Employment status**: Job stability or type of employment.
- **Loan details**: Such as loan term, requested amount, and interest rate.
- **Assets value**: A breakdown of residential, commercial, and luxury assets owned by applicants.
- **Loan status**: Whether previous applications were approved or rejected.

This dataset is widely used in machine learning projects focused on financial decision-making, helping to create predictive models that evaluate loan approval likelihood.

---

### **Data Cleaning Process** 🧹
To prepare the dataset for analysis, we performed several preprocessing steps:
1. **Column and Entry Cleanup**:
   - Eliminated leading and trailing spaces in column names and data entries to avoid inconsistencies during processing.
2. **Irrelevant Data Removal**:
   - Dropped the `loan_id` column as it added no value to predictive modeling.
3. **Consistency in Naming**:
   - Rechecked and sanitized entries to ensure uniformity throughout the dataset.

---

### **Feature Engineering** 🔨
To enhance the dataset's analytical value, new features were engineered:
- **`Total_Asset_Value`**:
  - This derived column aggregates the values of the following asset categories:
    - `residential_assets_value`
    - `commercial_assets_value`
    - `luxury_assets_value`
- These transformations not only made the dataset richer but also added predictive depth for modeling.

---

### **Encoding Categorical Variables**
Certain columns, such as `education` and `self_employed`, contained non-numeric data, which were converted into machine-readable formats:
- **One-Hot Encoding**: Used to convert categorical variables into dummy variables, ensuring these features could be effectively processed by machine learning models.
  
Additionally:
- **Normalization and Standardization**:
  - The dataset underwent both **Min-Max Scaling** and **Standard Scaling** to determine which preprocessing method led to better model performance.

---

## **Machine Learning Models** 🧠
We employed a variety of machine learning algorithms to create and test predictive models. Each model brought its unique strengths to the table:
1. **Logistic Regression**: A statistical method ideal for binary classification.
2. **K-Nearest Neighbors (KNN)**: A non-parametric method relying on proximity-based predictions.
3. **Decision Tree**: A rule-based approach offering interpretable and hierarchical decision-making.

---

## **Model Performances and Key Insights** 🗝️
Here are the results for each algorithm:

### **Logistic Regression**
- Normalized Model Performance:
  - **Accuracy**: 91.22%
  - **Precision**: 89%
  - **Recall**: 87%
  - **F1 Score**: 88%
  - **AUC-ROC**: 97%
- Strengths: Balanced performance across accuracy and precision metrics.

### **Decision Tree**
- Performance:
  - **Accuracy**: 97%
  - **Precision**: 98%
- Strengths: Outperformed other models with high accuracy and precision, making it the best fit for this problem.

### **K-Nearest Neighbors (KNN)**
- Normalized Model Performance:
  - **Accuracy**: 90%
  - **Precision**: 86%
  - **Recall**: 88%
  - **F1 Score**: 87%
- Strengths: Provided competitive results but fell slightly behind the Decision Tree.

---

## **Results** 📈
The evaluation highlighted the **Decision Tree** algorithm as the most effective for predicting loan approvals. While both Logistic Regression and KNN performed well, they were outshined by the Decision Tree model.

A significant finding was the pivotal role of the **CIBIL score**, which emerged as the most influential feature in determining loan approval outcomes.

---

## **Conclusion** ✔️
This project showcased how machine learning can revolutionize decision-making in the financial sector. By analyzing key features and leveraging powerful predictive models, we developed a robust solution that aids banks in assessing loan eligibility.

Looking ahead, future enhancements could include:
- Exploring more advanced algorithms like Random Forest or Gradient Boosting.
- Incorporating additional variables, such as macroeconomic factors.
- Enhancing model interpretability for better insights into decision-making.

## Datast Source:
https://www.kaggle.com/datasets/architsharma01/loan-approval-prediction-dataset 