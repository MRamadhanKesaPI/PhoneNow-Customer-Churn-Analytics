# PhoneNow: Customer Churn Analytics - PwC Switzerland Virtual Case Experience

**Welcome to my personal project repository!** 

## Table of Contents
- [**Project Background**](#project-background)
- [**Project Assets**](#project-assets)
- [**Data Structure**](#data-structure)
- [**Insights**](#insights)
- [**Recommendations**](#recommendations)


## Project Background

PhoneNow is a leading telecommunications company that provides mobile and internet services to a diverse customer base. With a strong market presence, the company has been focused on delivering high-quality services to retain customers and reduce churn. However, despite its efforts, PhoneNow has been experiencing a high churn rate, leading to customer losses and revenue impacts.

To address this challenge, PhoneNow has partnered with PwC Switzerland to uncover insights into customer churn patterns and identify strategies to improve retention. This analysis is based on customer churn data from the last month, providing the most up-to-date insights into recent trends and behaviors.


### Purpose of the Analytics Team:
The analytics team will focus on helping PhoneNow gain deeper insights into customer churn. The goals are to:

-  Identify the main factors driving churn and analyze their impact.
-  Understand customer trends to highlight opportunities for reducing churn.
-  Deliver recommendations to help PhoneNow enhance its retention strategies and improve long-term customer loyalty.


### Insight and Recommendation Focus:
The project focuses on providing actionable insights in these key areas:

1. **Churn Rate Analysis**,
identifying the overall churn rate and key patterns in customer losses.

2. **Contract Type Impact**,
evaluating how different contract types influence churn behavior.

3. **Tenure and Churn Relationship**,
analyzing customer lifecycle trends to determine when churn is most likely to occur..

4. **Service Usage Patterns**,
identifying services with high churn rates to pinpoint potential issues.

5. **Support Ticket Influence**,
assessing the impact of technical and administrative support on churn.


## Project Assets
To make the analysis and insights easy to explore, the following resources are available:

- The SQL queries for data preparation can be found [here](https://mramadhankesapi.github.io/Data-Preparation-Process_for_PhoneNow...Customer-Churn/).

- The DAX measures to support data analysis can be found [here](https://mramadhankesapi.github.io/DAX-Measures__for__PhoneNow...Customer-Churn/).
  
- A Power BI dashboard can be downloaded here: [PhoneNow Customer Churn.pdf](https://github.com/user-attachments/files/18759794/PhoneNow.Customer.Churn.pdf) or [PhoneNow Customer Churn.pbix](https://github.com/MRamadhanKesaPI/PhoneNow-Customer-Churn-Analytics/blob/main/PhoneNow%20Customer%20Churn.pbix)


## Data Structure
The PhoneNow database used in this project consists of three tables: Customer Churn, Service Type, and Bundle, with a total of 41,244 rows of data.

![Relationships PWC](https://github.com/user-attachments/assets/5aa5554e-ae2a-4afe-a194-c34d973793ba)

These final datasets were created through the process of creating view ini PostgreSQL, which can be found [here](https://mramadhankesapi.github.io/Data-Preparation-Process_for_PhoneNow...Customer-Churn/).

## Insights

#### 1. Churn Rate is High at 26.54%:
-  Over the last month, **one in four customers** have left PhoneNow, highlighting a significant churn issue. This rate suggests that **customer retention strategies need to be strengthened** to reduce further losses.
    
#### 2. Month-to-Month Customers Are the Most Likely to Leave:
-  Customers on **month-to-month** contracts accounted for **88.55%** of churn, compared to just 8.88% for one-year contracts and 2.57% for two-year contracts. This shows that **short-term customers are at the highest risk of leaving**.

#### 3. New Customers Churn the Most:
-  **55.48% of churned customers** left within their first 12 months.
-  Customers who **stayed longer (24+ months)** churned at much lower rates.
This indicates that early customer experience plays a crucial role in retention, and efforts should **focus on engaging and supporting new users**.

#### 4. Phone Service and Fiber Optic Customers Have Higher Churn:
-  Customers using **phone service** and **fiber optic internet** are more likely to churn. This suggests that these services might have quality or pricing concerns that need further investigation.

#### 5. Technical Issues Contribute to Churn Rather Than Administrative Issues:
-  **84.14%** of churned customers **had tech support tickets before leaving**. This means PhoneNow got a serious issues with tech.

---
Below is an overview from the Power BI dashboard. A Power BI dashboard can be downloaded here: [PhoneNow Customer Churn.pdf](https://github.com/user-attachments/files/18759794/PhoneNow.Customer.Churn.pdf) or [PhoneNow Customer Churn.pbix](https://github.com/MRamadhanKesaPI/PhoneNow-Customer-Churn-Analytics/blob/main/PhoneNow%20Customer%20Churn.pbix)

![PhoneNow Churn 1](https://github.com/user-attachments/assets/7e5eb567-839e-4403-8e28-ea3d203c6638)

![PhoneNow Churn 2](https://github.com/user-attachments/assets/129adfef-0540-4842-a6f3-c18c5e9d76ca)


## Recommendations

#### 1. Improve Retention for Month-to-Month Customers:
- Offer discounts, loyalty rewards, or upgrade incentives to encourage customers to switch to longer-term contracts. This could help reduce the high churn rate in this segment.
  
#### 2. Strengthen Early Customer Engagement: 
- Since over half of churned customers left in the last month were in their first year, focus on onboarding improvements, proactive customer check-ins, and personalized offers within the first 12 months.

#### 3. Investigate Phone Service and Fiber Optic Service Issues:
- Analyze customer complaints and gather feedback to understand why these services have higher churn. Consider improving service quality or offering better pricing plans.

#### 4. Enhance Technical Support Response Times:
- Technical issues might be the primary churn factor, faster and more efficient tech support could prevent some customers from leaving.

### Thank you for exploring this project, Feel free to hear your thoughts, insights, or any feedback! Let’s keep the discussion going!
