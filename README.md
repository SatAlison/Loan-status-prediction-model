# Loan Status Prediction

## Table of Contents
- [Project Overview](#project-overview)
- [Motivation and Objectives](#motivation-and-objectives)
- [Data Source](#data-source)
- [Tools](#tools)
- [Project Workflow](#project-workflow)
  - [Data Cleaning](#data-cleaning)
  - [Exploratory Data Analysis](#exploratory-data-analysis)
  - [Data Visualization](#data-visualization)
- [Insights and Recommendations](#insights-and-recommendations)
  - [Key Findings](#key-findings)
  - [Recommendations](#recommendations)
- [Limitations](#limitations)
- [Impact and Future Plans](#impact-and-future-plans)
- [References](#references)
- [Contact Information](#contact-information)


## Project Overview
The goal of this project is to develop a **machine learning model** to predict whether a loan will be **approved** or **denied** based on various factors. 
Additionally, the project aims to determine whether **log-transformed data** produces better results compared to the original data by analyzing and comparing the model's performance with both data types.


## Motivation and Objectives
The primary motivation for this project is to assist **financial institutions** in more accurately assessing loan approval risks. By predicting whether a loan will be **approved or denied**, lenders can improve portfolio management, reduce potential losses, and offer more tailored loan options to clients. 
Furthermore, this project explores the impact of using **log-transformed data** to determine if it enhances the model’s performance compared to using the original dataset.

## Objectives
- Analyze historical loan data to uncover trends and patterns.
- Identify key factors contributing to **loan approval** or **default**.
- Build a **predictive model** to forecast loan outcomes (approved or denied).
- Compare model performance to **choose the best model** for accurate loan prediction.
- Evaluate the impact of using **log-transformed data** versus original data on model accuracy.
- Test the model with **new data** to determine if a loan will be **approved or denied**.

## Data Source
The dataset used in this project contains records of past loans, including **demographic information**, **loan details**, and **borrower profiles**. The data was sourced from **Kaggle** as loan_prediction.csv' and can be accessed via the following link:[Kaggle Loan Dataset](https://www.kaggle.com/)

![Screenshot (34)](https://github.com/user-attachments/assets/8c3df74c-3ce1-41b1-bf34-2ba20c81d8ff)


## Tools
The following tools and libraries were used for data analysis, model development, and visualization:

**Python** for coding.
- `Pandas` for data manipulation.
- `NumPy` for numerical operations.
- `Scikit-learn` for machine learning models.
- `Matplotlib` / `Seaborn` for data visualization.
- **Jupyter Notebook** for interactive code development.


## Project Workflow

### Data Cleaning
- Handled missing values in key columns like `Loan Amount`, `Applicant Income`, and `Loan_Amount_Term`.
- Normalized and standardized numerical variables for consistent analysis.
- Categorical variables such as loan status were encoded to be used in machine learning models.

### Exploratory Data Analysis
- Explored distributions of key features such as loan amount, Gender, and Applicant Income.
- Visualized relationships between borrower attributes and loan outcomes to identify patterns.
- Transformed some data into a log scale using `np.log()` to achieve a normal distribution, specifically for columns like `Loan Amount` and `Total Income`.

![Screenshot (33)](https://github.com/user-attachments/assets/9a23153b-769d-42a4-a08a-a6ab4f7d89a2)

  
### Data Visualization
- Created histograms, box plots, and scatter plots to visualize the distribution of data.
- Used bar charts to display the proportion of loan status outcomes.

## Insights and Recommendations

### Key Findings

- Log-transformed data for income and loan amount provided a better distribution and improved prediction accuracy compared to the original data.
- **Logistic Regression** produced the best cross-validation scores before hyperparameter tuning for both the original and log-transformed data, and was therefore selected as the final model.
- The most important feature in the model is **credit history**, which had the strongest influence on the loan approval prediction.

![Screenshot (32)](https://github.com/user-attachments/assets/840453d6-e60d-4c44-9e7a-b38274f45147)


### Recommendations

1. **Focus on Credit History**:
   - Since credit history emerged as the most important feature in predicting loan status, financial institutions should prioritize assessing this aspect during the loan application process. Implementing stricter credit history evaluation criteria may reduce default rates.

2. **Utilize Log-Transformed Data**:
   - Given that log-transformed data for income and loan amounts improved prediction accuracy, consider incorporating log transformations in future analyses. This approach can help in modeling relationships that deviate from normal distributions.

3. **Enhance Data Collection**:
   - To further refine the predictive model, consider collecting additional demographic and financial data, such as:
     - Employment stability and job type
     - Existing debts and financial obligations
     - Savings and investment behavior

4. **Regular Model Updates**:
   - Implement a process for regularly updating the model with new data and retraining it to maintain accuracy. This will help in adapting to changing economic conditions and borrower behavior.

5. **Integrate Predictive Analytics into Decision-Making**:
   - Use predictive analytics to identify at-risk applicants early in the loan process. Implement risk mitigation strategies such as personalized loan terms or additional support for applicants with lower credit scores.

6. **Monitor External Factors**:
   - Keep an eye on economic indicators that may impact loan defaults, such as unemployment rates, inflation, and changes in lending regulations. Adjust lending strategies accordingly to mitigate risks associated with these factors.


## Limitations
- **Economic Changes**: The dataset may not reflect changes in the economy or regulations over time, which can affect loan outcomes.
- **Missing Data**: Gaps in important features could limit the model's accuracy and the reliability of the results. It's important to manage these missing values carefully.
- **Feature Selection**: The model may not include all relevant factors that influence loan status, which might oversimplify the issue.
- **Generalizability**: The results and model performance might not apply to all financial institutions or regions since different areas may have different characteristics and borrower behaviors.

## Impact and Future Plans
The model developed in this project can greatly help lenders predict loan defaults and improve their lending strategies. Future enhancements could include:
- **Using Updated Data**: Adding more recent information to better reflect current lending situations.
- **Including Additional Factors**: Incorporating external data, like credit scores or economic indicators, to boost the model's accuracy.
- **Testing Other Models**: Hypertuning different machine learning models to see if they perform better than the current one.
- **User-Friendly Interface**: Creating a simple interface for lenders to easily use the model in their decision-making process.

## References 
- Loan dataset from kaggle.
- Articles and tutorials on machine learning from You Tube.

## Contact Information
For any questions or further collaboration, please contact:
- **Name:** Satelite Alison Ndayikunda
- **Email:** [satalisonn@gmail.com](mailto:satalisonn@gmail.com)
