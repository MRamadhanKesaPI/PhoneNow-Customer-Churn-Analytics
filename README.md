# PhoneNow: Customer Churn Analytics - PwC Switzerland Virtual Case Experience

**Welcome to my personal project repository!** 

## Table of Contents
- [**Project Background**](#project-background)
- [**Project Assets**](#project-assets)
- [**Data Structure**](#data-structure)
- [**Insights (Power BI)**](#insights-power-bi)
- [**Predictive Insights (Logistic Regression - Python)**](#predictive-insights-logistic-regression---python)
- [**Recommendations**](#recommendations)


## Project Background

PhoneNow is a leading telecommunications company that provides mobile and internet services to a diverse customer base. With a strong market presence, the company has been focused on delivering high-quality services to retain customers and reduce churn. However, despite its efforts, PhoneNow has been experiencing a high churn rate, leading to customer losses and revenue impacts.

To address this challenge, PhoneNow has partnered with PwC Switzerland to uncover insights into customer churn patterns and identify strategies to improve retention. This analysis is based on customer churn data up to the last month, providing the most up-to-date insights into recent trends and behaviors.


### Purpose of the Analysis:
The goal of this analysis is focus on helping PhoneNow gain deeper insights into customer churn. The goals are to:

-  Identify the main factors driving churn and analyze their impact.
-  Understand customer trends to highlight opportunities for reducing churn.
-  Deliver recommendations to help PhoneNow enhance its retention strategies and improve long-term customer loyalty.


## Project Assets
To make the analysis and insights easy to explore, the following resources are available:

- The SQL queries for data preparation can be found [here](https://mramadhankesapi.github.io/Data-Preparation-Processes_for_PhoneNow...Customer-Churn/).

- The DAX measures to support data analysis can be found [here](https://mramadhankesapi.github.io/DAX-Processes__for__PhoneNow...Customer-Churn/).
  
- A Power BI dashboard can be downloaded here: [PhoneNow Customer Churn.pdf](https://github.com/user-attachments/files/19042483/PhoneNow.Customer.Churn.pdf) or [PhoneNow Customer Churn.pbix](https://github.com/MRamadhanKesaPI/PhoneNow-Customer-Churn-Analytics/blob/main/PhoneNow%20Customer%20Churn.pbix)

- The Python notebook for the Logistic Regression model can be found [here](https://github.com/MRamadhanKesaPI/PhoneNow-Customer-Churn-Analytics/blob/main/PhoneNow%20Customer%20Churn%20Prediction.ipynb).

## Data Structure
The PhoneNow database used in this project consists of three tables: Customer Churn, Service Type, and Bundle, with a total of 41,244 rows of data.

![Relationships PWC 1](https://github.com/user-attachments/assets/8c0132a4-f104-4350-8eb9-347eec43f063)

These final datasets were created through the process of creating view ini PostgreSQL, which can be found [here](https://mramadhankesapi.github.io/Data-Preparation-Processes_for_PhoneNow...Customer-Churn/).

## Insights (Power BI)

These insights serve as the foundation for the logistic regression model, which predicts future churn risks and identifies high-risk customers for proactive retention strategies.

### Key findings:
#### 1. Churn Rate is High at 26.54%:
-  Over the last month, **one in four customers** have left PhoneNow, highlighting a significant churn issue. This rate suggests that **customer retention strategies need to be strengthened** to reduce further losses.
    
#### 2. Month-to-Month Customers Are the Most Likely to Leave:
-  Customers on **month-to-month** contracts accounted for **88.55%** of churn, compared to just 8.88% for one-year contracts and 2.57% for two-year contracts. This shows that **short-term customers are at the highest risk of leaving**.

#### 3. New Customers Churn the Most:
-  **55.48% of churned customers** left within their first 12 months.
-  Customers who **stayed longer (24+ months)** churned at much lower rates.
This indicates that early customer experience plays a crucial role in retention, and efforts should **focus on engaging and supporting new users**.

#### 4. Some of Services Have Higher Churn:
-  Customers subscribed on **fiber optic internet**, **streaming tv**, **streaming movies**, **multiple lines**, and **phone service** and are more likely to churn. this suggests potential concerns with quality or pricing that require further investigation..

#### 5. Technical Issues Contribute to Churn Rather Than Administrative Issues:
-  **69.38%** of churned customers **had tech support tickets before leaving**. This means PhoneNow got a serious issues with tech.

---
Below is an overview from the Power BI dashboard. A Power BI dashboard can be downloaded here: [PhoneNow Customer Churn.pdf](https://github.com/user-attachments/files/19042483/PhoneNow.Customer.Churn.pdf) or [PhoneNow Customer Churn.pbix](https://github.com/MRamadhanKesaPI/PhoneNow-Customer-Churn-Analytics/blob/main/PhoneNow%20Customer%20Churn.pbix)


![Image](https://github.com/user-attachments/assets/3896a84c-4751-4981-b34d-11a75aa839c8)
![Image](https://github.com/user-attachments/assets/f5aa70c1-b3b1-4d08-ac14-0e3983c74a02)
---

## Predictive Insights (Logistic Regression - Python)

This model predicts customer churn using logistic regression, focusing on contract type, tenure, monthly charges, technical issues, and selected service subscriptions with the highest churn rates. The model calculates churn risk scores for every customers, helping identify high-risk customers and support better retention strategies. The full model implementation can be found [here](https://github.com/MRamadhanKesaPI/PhoneNow-Customer-Churn-Analytics/blob/main/PhoneNow%20Customer%20Churn%20Prediction.ipynb).

### Key findings:

#### 1. Strong Churn Detection (AUC-ROC: 0.92):
-  With an **AUC-ROC score of 0.92**, the model effectively distinguishes between churners and non-churners, ensuring reliable predictions.

![ROC Curve](https://github.com/user-attachments/assets/c0a75c41-b009-45db-a724-aa3c2c23c981)

#### 2. Model Predicts Churn with 80% Accuracy:
-  The model correctly classifies customers **80% of the time**, making it a solid predictive tool.

#### 3. High Recall for Churners (91%):
-  The model correctly identifies **91% of actual churners**, ensuring at-risk customers are flagged, though it may misclassify some loyal customers.

![Classification Report](https://github.com/user-attachments/assets/28f3defb-c354-464c-8cfb-e1251c63f7fb)

#### 4. 23.02% of Customers Are at Risk:
-  The model assigns churn risk scores to each customer, identifying **1,191 out of 5,174 active customers as high-risk**. Customers classified as high-risk have a **churn probability score above 50%**, reinforcing a **23.02% overall churn risk**.

![Churn Risk Above 50](https://github.com/user-attachments/assets/dc9ab2af-9a00-4128-895c-39af5dd6ed7f)


## Recommendations

#### 1. Improve Retention for Month-to-Month Customers:
- Offer discounts, loyalty rewards, or upgrade incentives to encourage customers to switch to longer-term contracts. This could help reduce the high churn rate in this segment.
  
#### 2. Strengthen Early Customer Engagement: 
- Since over half of churned customers left in the last month were in their first year, focus on onboarding improvements, proactive customer check-ins, and personalized offers within the first 12 months.

#### 3. Investigate Phone Service and Fiber Optic Service Issues:
- Analyze customer complaints and gather feedback to understand why these services have higher churn. Consider improving service quality or offering better pricing plans.

#### 4. Enhance Technical Support Response Times:
- Technical issues might be the primary churn factor, faster and more efficient tech support could prevent some customers from leaving.

---
### Thank you for exploring this project, Feel free to hear your thoughts, insights, or any feedback! Let’s keep the discussion going!
