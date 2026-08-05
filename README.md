# E-COMMERCE FUNNEL ANALYSIS

## Overview

The online retailer seeks to improve its sales performance by gaining a deeper understanding of customer behavior throughout the purchasing journey. This project analyzes e-commerce funnel data to evaluate how users progress from the homepage to checkout, with a focus on identifying conversion patterns and points of abandonment. The analysis examines customer behavior across different user types (New and Returning), traffic channels (Organic, Paid and Referral), and product categories. By identifying the stages with the highest drop-off rates and comparing conversion performance across key customer segments, the project provides actionable insights to help stakeholders optimize the user experience, improve marketing effectiveness, and increase overall conversion rates.

**Methodology:** A structured workflow was followed, covering data preparation, exploratory analysis, funnel analysis and dashboard development.

**Data Preparation:** The dataset was validated and prepared by resolving missing values, removing duplicates, correcting data types and standardizing categorical variables to ensure data quality and analytical accuracy.

**Exploratory Data Analysis:** Customer behaviour, user segments and traffic sources were explored using descriptive statistics and visualisations to understand user distribution and engagement throughout the purchasing funnel.

**Funnel Analysis:** Conversion rates were calculated at each stage of the customer journey (Home → Category → Product → Add to Cart → Checkout). Performance was then compared across user types, traffic channels and product categories to identify conversion patterns, quantify customer drop-offs and uncover opportunities to improve the purchasing experience.

**Dashboard Development:** An interactive Power BI dashboard was developed to present key performance indicators, funnel conversion metrics, segment comparisons and customer drop-off patterns, enabling stakeholders to monitor funnel performance and support data-driven decision-making.

## Business Understanding

In e-commerce, converting website visitors into paying customers is essential for driving revenue and business growth. This analysis evaluates how users progress through the purchasing funnel by measuring conversion rates between each stage of the customer journey and identifying where the largest drop-offs occur. By comparing funnel performance across user types, traffic channels and product categories, the project provides insights that help stakeholders optimize the customer experience, improve marketing effectiveness and increase overall conversion rates.

## Key Business Questions

**Funnel Performance:** How effectively does the e-commerce funnel convert users from the homepage to checkout?

**Customer Behaviour:** At which stage of the purchasing journey are the largest customer drop-offs occurring?

**User Performance:** How do conversion rates differ between new and returning users?

**Traffic Channel Performance:** Which traffic channels generate the highest-quality traffic based on conversion performance?

**Product Category Performance:** Which product categories achieve the highest and lowest conversion rates?

## Goal

The primary goals of this project are to:

- Measure conversion rates at each stage of the e-commerce purchasing funnel.
- Identify the stages where the largest customer drop-offs occur.
- Compare conversion performance across user types, traffic channels and product categories.
- Uncover patterns in customer behaviour that influence purchase completion.
- Provide actionable recommendations to optimize the customer journey and improve overall conversion rates.

## Data Source

The dataset contains customer interaction data captured across the e-commerce purchasing funnel. It includes information on user progression through each funnel stage (Home, Category, Product, Add to Cart and Checkout), along with user type (New and Returning), traffic channel (Organic, Paid and Referral) and product category.

## Tools & Technologies

**Python** – Processed, transformed, and analysed the e-commerce funnel dataset.

**Pandas & NumPy** – Performed data manipulation, aggregation, and numerical calculations to derive funnel metrics.

**Matplotlib** – Produced visualisations to examine conversion rates and customer drop-off patterns.

**Jupyter Notebook** – Supported data preparation, exploratory analysis, and project documentation.

**Power BI** – Built an interactive dashboard to communicate key performance metrics and business insights.

**Power Query** – Cleaned, validated, and prepared the dataset for dashboard reporting.

## Data Preparation

The dataset was prepared to ensure it was suitable for analysis and dashboard development.

### Data Loading

* Imported the e-commerce funnel dataset into Jupyter Notebook using Pandas.

### Data Inspection

* Reviewed the dataset structure, dimensions, data types, and checked for missing values and duplicate records.

### Data Cleaning

* Confirmed that the dataset contained no missing values.
* Retained duplicate session records, as they represented different stages of the customer journey within the same session.

### Feature Engineering

* Calculated session counts, conversion rates, and customer drop-off percentages to support the analysis.

### Data Integration

* Exported the prepared dataset as a CSV file for use in Power BI.

## Final Data
Following data preparation, the final dataset contained the key attributes required for funnel analysis and dashboard reporting, including: Session ID, User Type, Traffic Channel, Product Category, Funnel Page, Event Time, and Purchase Flag.

## Data Analysis and Visualization
The analysis examined overall funnel conversion performance, compared conversion rates across user types, traffic channels, and product categories, and identified the stages with the highest customer drop-off rates.

<img width="861" height="471" alt="image" src="https://github.com/user-attachments/assets/1ba6c9a9-5893-401a-9eb9-50748abd04fb" />

**Insight:**
Customer sessions decline steadily across the purchasing funnel, from 1,000 sessions at the Home page to 174 sessions at Checkout. The largest reduction occurs between the Product and Add to Cart stages, indicating a key point of customer abandonment. Overall, the funnel achieves a 17.4% conversion rate, highlighting opportunities to improve the customer journey and increase purchase completion.

<img width="573" height="514" alt="image" src="https://github.com/user-attachments/assets/022072b1-d866-4d14-abab-388b2e9b101a" />

The DataFrame is transposed (.T) so that the funnel stages appear on the x-axis while New and Returning users are displayed as separate bars within each stage.

**Insight:**
New and Returning users exhibit nearly identical conversion patterns throughout the purchasing funnel. While Returning users achieve a slightly higher overall conversion rate of 17.54%  than New users with 17.33%, the difference is minimal, suggesting that user type has little influence on conversion performance.

<img width="573" height="512" alt="image" src="https://github.com/user-attachments/assets/bb2cc392-9c52-486d-ac67-c1414248da7d" />

**Insight:**
Referral traffic demonstrates the strongest progression through most stages of the purchasing funnel, achieving the highest conversion rates from Category to Add to Cart. However, Paid traffic records the highest overall checkout conversion rate of 18.63%, while Organic traffic shows the lowest overall conversion of 16.40%, indicating potential opportunities to improve its purchase completion rate.

<img width="572" height="513" alt="image" src="https://github.com/user-attachments/assets/bf55459c-5be7-4de2-a664-b0c1e9c9c4ad" />

**Insight:**
The Bag category records the highest overall checkout conversion rate of 21.76%, followed by Jacket with 18.15%. In contrast, Shoes and Watch categories exhibit lower conversion rates, suggesting opportunities to improve customer engagement and purchase completion for these product categories.

<img width="688" height="463" alt="image" src="https://github.com/user-attachments/assets/adef3aee-40b8-430e-8d01-4d877e608ea4" />

**Insight:**
Customer drop-offs increase progressively as users advance through the purchasing funnel. The largest abandonment occurs at the Add to Cart stage, where 52.33% of sessions fail to proceed to checkout. This suggests that the transition from Add to Cart to Checkout is the primary bottleneck in the customer journey and should be prioritized for optimization.

## Dashboard Development

<img width="1048" height="587" alt="image" src="https://github.com/user-attachments/assets/6e6b912b-3ca3-4c24-b44a-549aff74bb92" />

**Analysis:**
The Power BI dashboard consolidates the key findings from the analysis into an interactive report, enabling stakeholders to monitor funnel performance and customer behaviour in a single view. It highlights the overall conversion funnel, customer drop-off rates, and conversion performance across traffic channels and product categories, providing a clear basis for identifying bottlenecks and supporting data-driven decision-making.

## Recommendations

1. Optimize the checkout process to reduce the high customer abandonment rate between the Add to Cart and Checkout stages.

2. Improve the Watch and Shoes product categories by enhancing their product pages, pricing strategies, and promotional efforts to increase conversions.

3. Allocate more marketing resources to Referral and Paid channels, as they demonstrated stronger conversion performance than Organic traffic.

4. Enhance product pages to encourage more users to progress from the Product stage to Add to Cart.

5. Continuously monitor funnel conversion metrics to identify emerging bottlenecks and support ongoing data-driven improvements.

## Conclusion

This project analysed the performance of an e-commerce purchasing funnel by evaluating user progression from the Home page to Checkout. The analysis revealed an overall funnel conversion rate of 17.40%, with customer sessions declining steadily at each stage. While conversion performance was broadly consistent across user types, differences were observed across traffic channels and product categories, providing valuable insights into customer behaviour.

The findings highlight opportunities to improve the customer journey, particularly by reducing abandonment between the Add to Cart and Checkout stages, strengthening lower-performing product categories, and leveraging high-performing marketing channels. By implementing these recommendations and continuously monitoring funnel performance, the business can enhance the customer experience, improve conversion rates, and drive sustainable sales growth.

## Github Link
https://github.com/gordon-moenga/Ecommerce-Funnel-Analysis
