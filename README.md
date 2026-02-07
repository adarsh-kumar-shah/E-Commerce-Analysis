# E-Commerce Data Analysis & Power BI Dashboard  
### Data-Driven Insights for Sustainable E-Commerce Growth
**By:** Adarsh Shah  

## Project Overview  
This project analyzes an e-commerce company’s operations to uncover insights that drive sustainable growth and customer satisfaction. Using data exploration, cleaning, and visualization techniques, it provides a comprehensive view of financial performance, customer behavior, product trends, and fulfillment efficiency. The insights were implemented into an interactive Power BI dashboard, supported by detailed Exploratory Data Analysis (EDA) in Python (Google Colab).  

## Objectives  
- Analyze financial performance and identify growth trends  
- Understand customer behavior and segmentation (B2B vs B2C)  
- Evaluate fulfillment performance (Amazon vs Merchant)  
- Study product demand and return patterns  
- Derive actionable recommendations for operational excellence  

## Problem Statement  
The company faces multiple challenges in managing:  
- Revenue growth and profit consistency  
- Order cancellations and returns  
- Fulfillment delays and channel dependencies  
- Inventory imbalance and category concentration  
- Customer retention and satisfaction  

**Goal:** Leverage data insights to optimize operations and ensure sustainable business growth.  

## Dataset Description  
| Column | Description |
|--------|-------------|
| Order ID | Unique identifier for each order |
| Date | Date of order placement |
| Status | Order status (Delivered, Cancelled, Shipped, etc.) |
| Fulfillment | Order fulfillment mode (Amazon / Merchant) |
| Sales Channel | Platform through which the order was made |
| Category | Product category |
| Size | Product size |
| Quantity | Number of units ordered |
| Amount | Total transaction amount |
| Ship-City/State/Country | Shipping location details |
| B2B | Boolean flag for B2B orders |
| Fulfilled By | Party responsible for shipping |

## Data Analysis Process  
### Step 1 – Data Exploration & Understanding
- Examined data structure, shape, and column consistency  
- Checked missing values and outliers  

### Step 2 – Data Cleaning
- Removed duplicates and invalid entries  
- Replaced missing values in the Amount column with median  
- Standardized date formats and category labels  

### Step 3 – Exploratory Data Analysis (EDA)
- Performed descriptive statistics and correlation analysis  
- Revenue trend visualization (monthly, category-wise)  
- Cancellation and return rate analysis  
- Fulfillment performance (Amazon vs Merchant)  
- Customer segmentation and city-wise revenue mapping  

### Step 4 – Dashboard Development (Power BI)
- Designed interactive visuals for financial KPIs, trends, and performance metrics  
- Applied DAX measures for:
  - Total Revenue = SUM(Sales[Amount])  
  - AOV (Average Order Value) = DIVIDE([Total Revenue],[Total Orders])  
  - Revenue Growth % = DIVIDE(([Total Revenue]-CALCULATE([Total Revenue],DATEADD(Sales[Date],-1,MONTH))),CALCULATE([Total Revenue],DATEADD(Sales[Date],-1,MONTH)))  
  - Cancellation Rate = DIVIDE([Cancelled Orders],COUNTROWS(Sales))*100

 ### Step 5 – Video Representation
- Created a PPT & Recorded a 7-minute video presentation explaining the dashboard design, and insights
- Highlighted challenges, methodology, and recommendations in a clear storytelling format

## Key Insights  
### Financial Performance
- Total Revenue: ₹71.84 M  
- Month-over-month growth: 42.87%  
- Highest revenue (₹26 M) in April  

### Customer Insights
- 99.3% B2C orders vs 0.7% B2B  
- Top 5 customers averaged 7–12 orders each  

### Product & Fulfillment
- “Set” and “Kurta” categories contribute ~76% of total revenue but show high cancellation rate (~16%)  
- Amazon fulfilled ~70% of orders, indicating operational dependency  

### Geographical Distribution
- Maharashtra and Karnataka lead with ~40% combined revenue  
- Bengaluru tops city performance with ₹6.8 M  

### Size Demand
- Medium (35%), Large (28%), and XL (22%) sizes account for 85% of total orders  


## Strategic Recommendations  
1. **Diversify Product Portfolio**  
   - Expand Western Dress and Ethnic Dress categories to reduce market risk  

2. **Optimize Fulfillment Channels**  
   - Aim for a 40–60 balance between Amazon and Merchant deliveries  

3. **Enhance Quality Control**  
   - Focus on high-return categories (Sets & Kurtas) with improved sizing and fabric information  

4. **Expand Geographical Reach**  
   - Target Tier-2 and Tier-3 cities with localized marketing campaigns  

5. **Inventory Alignment**  
   - Focus procurement on high-demand sizes (M, L, XL) to ensure efficient stock turnover  


## Tools & Technologies  
| Tool | Purpose |
|------|----------|
| Python (Colab) | Data Cleaning & EDA |
| Pandas, Matplotlib, Seaborn | Data processing & visualization |
| Power BI | Dashboard development & DAX measures |
| Excel | Data preparation & validation |
| Power Point | Presentation of Power Bi charts |
| GitHub | Version control & portfolio hosting |

## Project Components  
1. Google Colab Notebook – (https://colab.research.google.com/drive/1LbLRC6fm6lQOKSHE44RCHDqqP3ugIPwA?usp=drive_link)  
2. Power BI Dashboard (PPT Preview) – E-COMMERCE REPORT PRESENTATION.pptx  
3. Problem Statement Document – Problem Statement.pdf  
4. Video Presentation – (https://drive.google.com/file/d/1kwvDTH-GzbrC7G2YIu3SVd_0purWHCbo/view?usp=drive_link)
5. Power BI file - E-Commerce Sales Dashboard

## Project Outcomes  
- Provided complete business visibility through a unified dashboard  
- Delivered actionable insights for marketing, inventory, and logistics  
- Enabled data-driven strategic decision making for sustainable growth  
- Strengthened BI, EDA, and storytelling skills using Power BI and Python  

