# Retail Customer & Sales Analysis

## 📌 Project Overview

This project is an end-to-end Exploratory Data Analysis (EDA) of retail customer data. The objective was to clean, explore, visualize, and statistically analyze customer characteristics, purchasing behaviour, satisfaction, and Customer Lifetime Value (CLV).

The analysis was carried out using Python, with the results translated into data-driven insights and recommendations that could support business decision-making.

## 🎯 Business Objective

The analysis focused on answering key business questions:

- What are the characteristics of the company's customers?
- How does customer income vary across regions?
- How does age relate to purchasing behaviour?
- What factors are associated with Customer Lifetime Value?
- Is there a relationship between income and customer satisfaction?
- Does customer income differ significantly between highly satisfied and less satisfied customers?
- What actions can the business take to improve customer retention and value?

  ## 🛠️ Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
- Jupyter Notebook

## 🧹 Data Cleaning & Preparation

The dataset was prepared for analysis by:

- Checking for duplicate records and removing duplicates where necessary.
- Identifying missing values in the dataset.
- Handling missing values in the `Income` column using median imputation.
- Reviewing the data types and structure of the dataset.
- Creating a new Customer Lifetime Value (CLV) variable to support customer value analysis.

### Customer Lifetime Value (CLV)

CLV was calculated using:

**CLV = Purchases × Member_Years × 15**

The CLV metric was used to estimate the potential long-term value of each customer.

## 🔍 Exploratory Data Analysis

The cleaned dataset was explored to understand customer characteristics,
purchasing behaviour, satisfaction, and customer value.

### Regional Analysis

Average Income and Average Satisfaction were calculated for each region
using GroupBy operations.

This helped identify differences in customer characteristics across the
North, South, East, and West regions.

### Age & Purchasing Behaviour

Customers were grouped into three age categories:

- Under 30
- 30–50
- Over 50

A pivot table was used to examine average Purchases across different
regions and age groups.

A scatter plot was also created to investigate the relationship between
Age and Purchases, with customers differentiated by Region.

### Customer Lifetime Value

Customer Lifetime Value (CLV) was analyzed alongside Member_Years to
understand whether longer-term customers tend to generate greater value
for the business.

## 📊 Visualizations

Two key visualizations were developed to communicate the findings:

### 1. Average Income by Region

A bar chart was used to compare average customer income across the
different regions.

### 2. Age vs Purchases

A scatter plot was used to examine the relationship between customer age
and number of purchases. Customers were differentiated by region to
identify potential regional patterns.

The visualizations were combined into a single figure to provide a
compact view of the analysis.

## 📈 Statistical Analysis

### Correlation Analysis

Correlation analysis was used to examine relationships between key
customer variables.

- **Income vs Satisfaction:** -0.013
- **Member_Years vs CLV:** 0.756

The Income–Satisfaction correlation indicates virtually no linear
relationship between income and satisfaction.

The positive correlation between Member_Years and CLV indicates a strong
positive relationship, suggesting that customers with longer membership
tend to generate higher lifetime value.

### Independent-Samples T-Test

An independent-samples t-test was used to compare the average income of
customers with:

- Satisfaction score ≥ 7
- Satisfaction score < 7

**T-statistic:** -0.213  
**P-value:** 0.8315

Since the p-value is greater than 0.05, the difference in income between
the two satisfaction groups was not statistically significant.

## 💡 Key Insights

1. Customer income showed virtually no linear relationship with
   satisfaction.

2. Member_Years and CLV showed a strong positive relationship,
   indicating that longer-term customers tend to generate greater
   lifetime value.

3. The statistical test found no significant difference in income
   between highly satisfied customers and customers with lower
   satisfaction scores.

4. The Age vs Purchases visualization showed no clear trend, suggesting
   that age alone is not a strong predictor of purchasing behaviour.

   ## 🎯 Business Recommendations

### 1. Strengthen Customer Retention

Since longer membership is strongly associated with higher Customer
Lifetime Value, the company should invest in loyalty programmes,
personalized rewards, and retention campaigns to encourage long-term
customer relationships.

### 2. Focus on Customer Experience

Since income showed virtually no relationship with customer
satisfaction, the company should focus on improving product quality,
customer service, and personalized engagement rather than targeting
customers based primarily on income.

## 📁 Project Files

- 📓 [View Python Analysis Notebook](Retail_Customer_Analysis.ipynb)
- 📊 [View Project Visualization](capstone_dashboard.png)
- 📄 [View Project Report](Retail_customer_Analysis_Report.pdf)
