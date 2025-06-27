# Super-Store-Sales-Deep-Analysis-Power-BI-Portfolio-Project

## Executive Summary
This project delivers a comprehensive business intelligence solution for a global superstore’s sales, profitability, and operations. From raw data cleansing and advanced Power Query transformations to custom DAX measures, star-schema modeling, and highly actionable dashboard design, every step was engineered to support real-world executive decision-making and drive business outcomes.

## Data Workflow & Modeling

**Data Sources:** Integrated Orders, People, Returns, Customer RFM tables (with “Final Fact Table” as the enriched fact dataset).

**Data Cleaning & Preparation:**

Removed nulls, fixed data types, handled duplicates, normalized categorical fields.

**Created key engineered columns**: Ship Duration, Profit Margin, IsReturned, Year-Month, and custom flags for advanced segmentation.

**Merging & Relationships:**

![image](https://github.com/user-attachments/assets/b93c3409-1bf7-475e-bbfb-575d5880feea)

Performed complex merges (joins) in Power Query to enrich facts with returns and region manager data.

Modeled all tables in a clear star schema for scalable analysis.

**Custom DAX & Measures:**

Built a wide set of DAX measures and columns (CLV, Churn Rate, Repeat Customer Rate, Discount Sensitivity, RFM Segmentation, Shipping Cost KPIs, Return Rates, etc.).

Constructed calculated columns for advanced date hierarchies and performance tracking.

## Analytical Dashboards & Key Insights
## 1. Executive Overview

![image](https://github.com/user-attachments/assets/74ceb981-98f5-490a-85c8-ddfd6b1e9f4b)

**Market Distribution & Risk**
Revenue is highly concentrated in a few key countries like U.S, India, Australia, France, and China account for the majority of sales. This creates both a scaling opportunity (by doubling down on proven markets) and a market concentration risk if demand drops or competition rises in any of these countries. Markets such as France and China are especially notable for their high sales volumes but show slightly lower profit margins, likely due to shipping costs or competitive pricing.

**Long Tail Potential**
Many markets—visible in the “Top Markets” donut—contribute only marginally to total revenue. There is untapped growth potential in these lower-volume countries, which could be realized via targeted marketing or tailored product bundles.

**Top Products & Customers**
Product Revenue Leaders: 3D printers (e.g., GBC Ibimaster 500), imaging and office equipment dominate top-selling products, suggesting a skew towards technology and office supply categories.
Key Customer Segments: The top five customers contribute a significant share of revenue, underlining the importance of key account management and retention strategies.

## 2. SUPER STORE SALES & PROFITABILITY

![image](https://github.com/user-attachments/assets/0da64d89-59ba-481c-b542-860ac812876b)

### Key Insights & Analysis

**1. Segment Profitability**

Consumer Dominance: The Consumer segment consistently delivers the highest profit, nearly doubling the next best (Corporate), especially in later years. This highlights a strong product-market fit and brand resonance with end-consumers.

Corporate & Home Office: While Corporate shows steady growth, Home Office remains the smallest and slowest-growing segment, suggesting an opportunity for repositioning or product line review.

**2. Profitability by Product Category**

Technology Leads: Technology is the profit engine, followed by Office Supplies, with Furniture lagging. Margins in Technology are likely buoyed by high-ticket items and less price sensitivity.

Strategic Focus: Shifting marketing spend or inventory towards top-performing categories may unlock additional margin.

**3. Profitability by Region**

Geographic Winners & Laggards: Profitability varies sharply by region, with certain geographies (e.g., India, Australia) outperforming others in both total profit and margin. Regional cost structures, logistics, and local competition likely drive this divergence.

**4. Discount Sensitivity**

Discount vs. Profit: The scatter plot clearly shows a negative correlation between high average discounts and lower average profit per product, especially in Office Supplies. Discounting is an effective demand lever but may erode profitability if not carefully targeted.

## 3. CUSTOMER INSIGHTS

![image](https://github.com/user-attachments/assets/d548b1ab-3bf4-4c67-85f2-f390c2d12d4d)


### Key Insights & Analysis

**1. Customer Base Composition**

**Repeat Customer Rate:** Only 16.58% of customers are repeat buyers, and 491 customers have placed more than one order. This suggests substantial room to improve retention via loyalty programs or targeted outreach.

**Churn Analysis:** The churn rate sits at 4.27%, highlighting a relatively stable but improvable customer base.

**2. Customer Lifetime Value (CLV)**

**Average CLV:** $569.62

Indicates a high spending per retained customer, which validates investments in relationship marketing and after-sales service.

**3. RFM Segmentation**

**Lost Customers:** Only 3.85% of customers are flagged as "lost"—a strong signal of healthy customer lifecycle management.

**Segment Sales Distribution:** The Consumer segment accounts for nearly 50% of sales, with Corporate and Home Office splitting the remainder. Tailoring offers and communications by segment could drive further loyalty.

**4. Returns by Customer**

Returned Orders: A handful of customers (e.g., Bart Pistole) are responsible for a disproportionate number of returns. This provides an opportunity for direct engagement to understand dissatisfaction and reduce future returns.

## 4. PRODUCT PERFORMANCE

![image](https://github.com/user-attachments/assets/c795d7a7-784a-4303-b3c6-8aed3ec400f5)

### Key Insights & Analysis

**1. Sales by Category & Sub-Category**

Tech and Office Supplies Dominate: Both categories, especially sub-categories like Phones, Copiers, and Appliances, drive the bulk of sales, while Art and Envelopes are clear laggards.

**2. Top Products**

**Concentration:** The top five products contribute a significant portion of total sales, suggesting a winner-takes-most dynamic and potential supply chain leverage for these SKUs.

**3. Product Discount Sensitivity**

**Vulnerability:** Certain high-selling products are more sensitive to discounts, exhibiting sharp margin erosion when discounting is aggressive.

**Pricing Levers:** Selective discounting and price optimization could materially boost overall margin.

## 5. GEOGRAPHICAL PERFORMANCE

![image](https://github.com/user-attachments/assets/13229ab7-c8d6-4699-bfb0-f47d33a4ba41)

### Key Insights & Analysis

**1. Market Performance**

India and Australia: Consistently top the sales charts, with France, China, and a handful of others following.

Low-Performing Markets: Several regions contribute minimally to both sales and profit, representing future expansion or exit decisions.

**2. Shipping Cost vs. Sales**

Correlation: In most regions, higher shipping costs are justified by higher sales—though certain outliers indicate inefficiency or opportunities for logistics improvement.

**3. Regional Profitability Leaders & Laggards**

Southern Africa, North Africa, Caribbean: These regions achieve above-average profit margins, likely due to favorable cost structures or niche market positioning.

Western Europe and Western Africa: Margins are notably lower, requiring investigation into local competition, cost, or pricing issues.

## 6. RETURNS & LOSS ANALYSIS

### Key Insights & Analysis

**1. Return Rate**

Acceptable Threshold: Overall return rate is 4%, well below the 9% acceptable threshold, reflecting healthy operations and effective product quality controls.

**2. Loss from Returns**

Technology Hit Hardest: Technology products drive the largest dollar loss from returns, indicating either product complexity or post-sale dissatisfaction.

Furniture and Office Supplies: Lower return losses, suggesting better fit or simpler logistics.

**3. Returns by Category and Market**

Regional Variance: Certain regions and categories have much higher return rates, highlighting the need for region- and product-specific return management strategies.

## 7. OPERATIONAL ANALYSIS

![image](https://github.com/user-attachments/assets/db6dd374-ce86-4fba-94d3-6fb48e87ac93)

## Key Insights & Analysis

**1. Avg. Ship Time by Ship Mode**

Standard Class Lags: Standard Class is the slowest fulfillment method, with Same Day and First Class performing best. Tradeoffs between cost and speed should be considered for margin improvement.

**2. Order Priority vs. Profit**

Medium Priority Wins: Medium-priority orders deliver the highest profit, while low-priority orders contribute the least. Operational focus on optimizing fulfillment for high- and medium-priority orders is warranted.

**3. Lead Time Analysis**

Distribution: The majority of orders are shipped within 4 days, but there are long-tail outliers that may indicate process bottlenecks or exceptions.

**4. Critical Orders**

Exception Management: A set of orders account for outsized sales, profit, or delays—requiring special monitoring for business continuity.

## Strategic Recommendations & Optimization Opportunities

Based on the comprehensive analysis, **Super Store** should focus on the following areas to drive sustainable growth and long-term profitability:

---

### 1. Enhance Profitability Through Product Mix and Margin Optimization

- **Observation:** Technology and Office Supplies drive most profits, while discounting erodes margins in several categories.
- **Recommendation:**
  - Refocus inventory and marketing on the most profitable categories and SKUs.
  - Implement dynamic pricing strategies to reduce unnecessary discounting, especially for in-demand products.
  - Use targeted promotions for slow-moving or low-margin products to boost turnover without sacrificing profitability.

---

### 2. Boost Customer Retention and Lifetime Value

- **Observation:** Repeat customers represent only ~17% of the base but have a much higher CLV.
- **Recommendation:**
  - Launch loyalty or referral programs to encourage repeat purchases.
  - Use RFM segmentation to tailor communications and offers to high-value and at-risk customers.
  - Monitor churn risk proactively and engage customers with high return rates or declining order frequency.

---

### 3. Reduce Returns and Associated Losses

- **Observation:** Return losses are highest in Technology, with some customers repeatedly returning products.
- **Recommendation:**
  - Conduct root-cause analysis for returns by product and customer segment.
  - Improve post-sale support and provide clear product information, especially for complex products.
  - Consider differentiated return policies based on product category and customer profile.

---

### 4. Improve Operational Efficiency in Shipping and Fulfillment

- **Observation:** Standard Class shipping is the slowest, and fulfillment delays can impact customer satisfaction and profit.
- **Recommendation:**
  - Optimize logistics for faster, more reliable delivery, especially for high-priority and high-value orders.
  - Regularly review the cost-benefit balance between shipping speed, cost, and customer value.
  - Establish real-time monitoring and escalation protocols for critical or delayed orders.

---

### 5. Leverage Data-Driven Decision Making

- **Observation:** The new analytics dashboards provide deep and actionable insights.
- **Recommendation:**
  - Institutionalize monthly executive reviews of key metrics and trends.
  - Foster collaboration between sales, marketing, operations, and customer service teams using shared insights.
  - Continuously iterate on analytics models and reporting to answer new business questions and identify emerging opportunities.

---

**Summary:**  
By prioritizing margin optimization, customer loyalty, return reduction, operational agility, and market expansion, Super Store can turn analytics into sustainable business impact.

 - [Super Store Interactive Dashboard (Power BI)]([https://github.com/movet306/Walmart-Sales-Analysis/blob/main/Walmart%20Sales%20Forecasting%20(1).ipynb](https://github.com/movet306/Super-Store-Sales-Deep-Analysis-Power-BI-Portfolio-Project/blob/main/SuperSales%20Deep%20Analysis.pbix))

**Please click on 'View Raw' to display and download the Power BI document**

Data Source: https://powerbidocs.com/tag/sample-superstore-sales-excel-xls/?ref=hackernoon.com 

