# Machine Learning-Based Optimization of US Car Insurance Premiums

## Project Overview
This project aims to analyze factors that influence the total claim amount in car insurance accidents by leveraging two datasets from different insurance companies. Using predictive modeling techniques such as Linear Regression, Decision Tree, and Naive Bayes, the analysis explores the relationship between key variables, including vehicle age, customer characteristics, and policy details, to predict claim amounts.

This study focuses on **U.S. car insurance claim amount prediction**, and it is critical for several reasons:

1. **Pricing**: Accurate claim predictions help insurance companies set yearly premiums effectively.
2. **Cash Reserves vs. Investment Capital**: Precise predictions allow companies to allocate cash reserves appropriately, optimizing investments for higher profitability.
3. **Profitability vs. Coverage**: Predictive insights help insurers maintain a balance between competitive pricing, profitability, and adequate coverage for policyholders.

By analyzing policyholders' demographic data and accident details, we aim to provide insurance companies with insights that can optimize pricing strategies, balance risk with profitability, and ensure fairness for customers.

## Problem Statement
Insurance companies face challenges in ensuring profitability while offering competitive and fair premiums to policyholders. One critical aspect is accurately predicting car insurance claim amounts, which depend on various factors like the age of the vehicle, customer demographics, and policy features.

The ability to predict claim amounts is crucial for the following reasons:
1. It helps insurance companies set competitive yearly premiums.
2. Accurate predictions assist companies in managing cash reserves while optimizing investment capital for better returns.
3. Competitive analysis of claim predictions ensures that companies remain profitable while providing adequate coverage for policyholders.

By understanding these factors, companies can better set premiums, categorize high-risk policies, and maintain a balance between profitability and customer satisfaction. This study, based on two datasets, compares the performance of various predictive models and parameter settings, offering valuable insights for the insurance industry.


## Dataset Description

This project utilizes two datasets from different insurance companies to analyze and predict car insurance claim amounts. Below is a brief overview of the key features and structure of each dataset:

### Main Features Across Datasets:
- **Monthly Premium**
- **Age**, **Gender**, **Income**
- **Employment Status**
- **Vehicle Size**, **Car Make**
- **Number of Vehicles**
- **Location**
- **Coverage Type**

### Dataset 1:
- A simpler dataset containing **24 columns** and over **9,000 rows**.
- **No missing data** and all features are well-structured for analysis.

### Dataset 2:
- A more complex dataset with **over 40 columns** and around **1,000 records**.
- Contains some **irrelevant** and **missing data**, requiring more preprocessing before analysis.

Both datasets focus on policyholder information, vehicle details, and coverage types, providing a solid foundation for exploring predictive models and premium optimization.


## Methodology & Results

We applied three predictive models: **Linear Regression**, **Decision Tree**, and **Naive Bayes** across both datasets. Initially, Linear Regression yielded an R² value of 72% for Dataset 1, indicating moderate prediction accuracy. In contrast, Dataset 2 achieved a significantly higher R² of 96%, suggesting a strong fit between the model and the actual claim amounts.

To improve model performance, we conducted feature importance analysis to identify key relationships between variables. For Dataset 1, we observed non-linear patterns, which the Linear Regression model struggled to capture. Switching to Decision Tree models, we saw improvements, with R² scores of 81% for Dataset 1 and 96% for Dataset 2. By tuning hyperparameters such as **Maximum Depth** and **Minimum Samples Split**, we further enhanced the model’s accuracy.

The performance difference between datasets is likely due to Dataset 2 containing more numerical features, which offered richer information for the models to generalize effectively.

Finally, the **Naive Bayes** model outperformed both regression models, delivering precision scores of 94% for Dataset 1 and 96% for Dataset 2. Naive Bayes was particularly well-suited for this problem, as it focuses on binary classification, where the outcomes are more discrete and align with the model’s strengths. Additionally, weak correlations in the datasets aligned well with the Naive Bayes assumptions, making it a highly effective approach.

## Final Conclusion and Business Insights

Through our analysis of the two datasets, we found that not all policyholder features significantly impact claim predictions. However, vehicle information—such as price and brand—and accident details, including the type of accident, time, and the number of vehicles involved, have a strong influence on the claim amount.

An important insight is the causation relationship between variables. For example, in Dataset 1, the "monthly premium" appears to be a strong predictor, but it's likely influenced by past claims, which introduces potential biases in some models that assume independence between variables.

For insurance companies, understanding these key factors is crucial for accurate predictions and better underwriting. By focusing on these major predictors, insurers can enhance risk management, refine pricing strategies, and set more precise underwriting criteria, ultimately improving profitability and operational efficiency.

### Major Features
- **Dataset 1**:  
  - Monthly Premium Auto  
  - Coverage  
  - Vehicle Class  
  - Location  

- **Dataset 2**:  
  - Number of Vehicles in Accident  
  - Location  
  - Incident Date  
  - Car Make  

### Minor Features
- **Dataset 1**:  
  - Age  
  - Education Level  
  - Gender  

- **Dataset 2**:  
  - Age  
  - Education Level  
  - Gender  

By prioritizing these features, insurance companies can more accurately predict claim amounts and adjust their underwriting and pricing strategies accordingly.


## Authors
- Beilin Ye [GitHub Profile](https://github.com/BeilinYe)
- Harneet Kaur
- Lida Ghasemi
