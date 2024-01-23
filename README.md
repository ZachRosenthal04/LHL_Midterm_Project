# LHL_Midterm_Project/Tequila Sales Data Analysis Project

## Disclaimer

The information provided in this repository has been altered to protect the company's intellectual property. Specific product names (SKUs) and certain financial figures have been slightly modified. While these changes do not affect the overall patterns and insights derived from the data analysis, they ensure that sensitive business information remains confidential.

## Introduction

A tequila company has amassed an extensive collection of sales data from its global market operations. This project aims to steer the company toward a data-centric approach, transforming raw data into strategic insights that drive business decisions.

## Problem Statement

The company boasts an array of tequila products and a substantial market presence. However, the absence of a data-driven framework has led to underutilized sales data. The project seeks to address critical challenges:

- Identifying the most lucrative markets and products.
- Assessing the impact of marketing strategies and brand ambassador engagements.
- Optimizing pricing to improve profit margins.
- Targeting sales efforts to boost the monthly sales rate per account.

The outcomes of this project are pivotal for developing an informed sales strategy.

## Industry-Specific Challenges

Tequila, as a controlled substance, presents distinct challenges in the market. The United States enforces a three-tier system separating production, distribution, and retail, while Canadian provinces maintain their own regulatory controls. For the company, it is imperative to:

- Adhere to the legal frameworks of federal and provincial laws.
- Plan strategically for market entry and growth.
- Align marketing strategies with regional regulations.
- Streamline supply chain management for cost-efficiency and effectiveness.

The data analysis incorporates these regulatory elements to provide compliant and insightful results.

## Dataset Description

This section details the various data points collected by the company, reflecting sales performance, market segmentation, and operational metrics.

### SKU Information
- **Basic SKUs**: The core products of the company.
  - *Tequila Plata*
  - *Tequila Reposado*
  - *Tequila Anejo*
- **Luxury SKUs**: Premium products with superior quality, packaging, and price. Introduced to the markets in late 2022.
  - *Tequila Supremo*
  - *Tequila Wooden Cask*
  - *Tequila Vivo*

### Sales and Market Data
- **Country**: The country where products are sold.
- **State/Province/Market**: Specific market within the country.
- **Year**: The year when sales occurred.
- **Month**: The month when sales occurred.
- **Full Date**: The exact date of the recorded sales data.
- **Market Manager**: The individual managing the respective market.

### Financial Metrics
- **Cost of Goods Sold**: The production cost for the products.
- **Sell Price**: The wholesale price at which goods are sold.
- **Profit**: Earnings calculated from the cost and sell price.
- **Profit Margin**: The percentage of profit in relation to the sell price.
- **Sales (4.5 L Cases)**: Monthly sales volume in the market, measured in 4.5-liter cases.
- **Revenue from Sales**: Total revenue generated from monthly sales.
- **Profit of Sales**: Profit derived from sales in that month.
- **Accounts Sold**: The number of accounts to which the company sold products in that month. The company only started tracking this metric in 2023 and only in markets where the distributor's system is capable.
- **Monthly Rate of Sales per Account**: The sales rate, based on the volume sold and the number of accounts.

### Marketing and Distribution Data
- **Number of Tequila Tastings/Samplings**: The count of marketing events like tastings/samplings conducted.
- **Distributor Size**: Categorized as Large, Medium, or Small, based on the volume they manage as whole in the market.
- **Market Type**: Classified as Free Market or Controlled Market.
- **Brand Ambassador Hired**: Indicates whether a brand ambassador was employed (Yes/No).
- **Number of Brand Ambassadors**: The total count of brand ambassadors engaged.
- **Top 10 Tequila Market**: Specifies if the market is among the top 10 for tequila sales (Yes/No).

## Data Analysis

### Data Integration and Standardization

The initial stage involved consolidating data from multiple reporting systems that used different units of measurement, such as 9L cases, 4.5L cases, or individual bottles. The company standardizes data to 4.5L cases (6x750ml bottles) to reflect its product packaging standards. This standardization is crucial for:

- Maintaining data consistency across analyses.
- Enabling precise comparisons across diverse data sets.
- Laying a dependable groundwork for actionable insights.

### Exploratory Data Analysis (EDA)

The EDA is executed in a Jupyter Notebook, with a focus on:

- **Data Cleaning:** Rectifying issues like missing values, duplicates, and inconsistencies.
- **Data Transformation:** Modifying data structures for analysis, including normalization and aggregation.
- **Statistical Analysis:** Applying descriptive statistics to understand the data's properties.
- **Correlation Analysis:** Exploring relationships within the data to guide sales strategy formulation.

### Data Visualization with Tableau

Tableau's powerful visualization tools are employed to:

- Construct interactive dashboards for immediate insight access.
- Generate clear visualizations that convey complex data to a broad audience.
- Provide dynamic filtering options for a personalized analysis experience.

## Dashboard User Guide

### Visualizations

#### 1. Interactive Map of North American Markets
- **Function:** Displays each market in North America.
- **Details on Hover:**
  - Market/State/Province name.
  - Total case sales in 4.5L units.
  - Revenue and profit figures in dollars.

#### 2. Bar Chart: Top Markets by Case Sales and Revenue
- **Purpose:** Showcases leading markets by case sales and revenue.
- **Features:** Comparative view of top performing markets.

#### 3. Line Chart: Monthly Case Sales Trends
- **Function:** Presents monthly case sales data.
- **Insights:** Visualizes trends and seasonal sales variations.

#### 4. Multi-Level Bar Chart: Market Manager Performance by SKU
- **Details:** Breakdown of performance by Market Manager.
- **Data Displayed:** Each manager’s sales figures by SKU.

### Filters for Custom Analysis

- **SKU:** Focus on specific product lines.
- **Year:** Select the year for sales data.
- **Quarter:** Choose a specific quarter for detailed insights.
- **Market Manager:** View data for a specific manager's region.

## Key Findings from Data Analysis

### Top 5 Markets by Case Sales and Revenue
Our analysis revealed the top-performing markets in terms of case sales and revenue:

1. **Ontario, Canada**: Leading with over 8,500 cases sold and revenue exceeding 1 million dollars.
2. **Georgia, USA**: Follows closely with 7,500+ cases and over $950,000 in revenue.
3. **California, USA**: Shows strong performance with 5,500+ cases and $750,000+ in revenue.
4. **Florida, USA**: Records sales of 5,000+ cases and revenue around $699,000.
5. **Oklahoma, USA**: Contributes significantly with 4,000+ cases and $480,000+ in revenue.

These markets are pivotal for our strategic focus and resource allocation.

### Most Profitable Products
- **Tequila Vivo**: Despite lower sales volume (731 cases), it's the most profitable per case, averaging $308 profit per case.
- **Tequila Plata**: This product stands out for its high volume sales (32,000+ cases), offsetting its lower profit per case of $59.91.

Understanding product profitability helps in prioritizing production and marketing efforts.

### Seasonal Sales Peaks
Our analysis highlights clear seasonal trends in tequila sales:
- **Q1 Slump**: Sales drop consistently in Q1 (January to March).
- **Pre-Cinco de Mayo Rise**: A significant sales increase is observed before Cinco de Mayo.
- **Summer Slight Increase**: Sales moderately rise during summer months.
- **OND Boost**: A notable surge in sales during the "OND" months (October, November, December), aligning with the holiday season.

This seasonality guides our marketing and stock planning.

### Impact of Tequila Tastings/Samplings on Sales
- **Direct Correlation**: The regression analysis shows a significant impact of tastings on sales, with a P-Value < 0.0001. An increase of 3.56 cases sold is observed for every tasting event conducted.

This insight emphasizes the importance of tastings as a tool to boost sales.

### Impact of Brand Ambassadors on Sales
- **Positive Influence**: The presence of Brand Ambassadors correlates strongly with increased sales (P-Value < 0.0001). On average, markets with Brand Ambassadors see an increase of 11.58 cases sold per month.

The data underscores the value of investing in Brand Ambassadors as part of our marketing strategy.

## Conclusion

Through thorough data analysis and the development of accessible visualizations, the project facilitates a transition to data-driven decision-making for the company, ensuring adherence to industry regulations and navigating through the intricacies of data integration.
