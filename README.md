# Jumia Product Performance Dashboard

## Project Overview

This project analyzes Jumia product data using Microsoft Excel to understand product pricing, discounts, customer reviews and ratings.

The objective was to transform raw e-commerce product data into a cleaned, analyzed and interactive Excel dashboard that can help sellers understand product performance and make better pricing and marketing decisions.

## Project Objectives

The project aimed to:

* Clean and prepare the Jumia product dataset.
* Analyze current and old product prices.
* Calculate and analyze discounts.
* Examine customer review counts and ratings.
* Identify high-performing and underperforming products.
* Analyze the relationship between discounts, reviews, ratings and prices.
* Build an interactive Excel dashboard.
* Develop evidence-based business insights and recommendations for Jumia sellers.

## Dataset

The dataset contains Jumia product information with the following main fields:

* Product
* Current Price
* Old Price
* Discount
* Review
* Rating

The original dataset contained 115 records. After removing duplicate records, the cleaned dataset contained **112 products**.

## Data Cleaning

The following data-cleaning activities were performed:

### 1. Duplicate Removal

Duplicate records were identified and removed to prevent repeated products from distorting the analysis.

Three duplicate records were removed.

### 2. Review Cleaning

Some review values appeared as negative numbers. Since customer review counts cannot logically be negative, the values were converted to their absolute values.

Blank review values were retained as missing rather than automatically being converted to zero.

### 3. Rating Cleaning

Rating values were converted from text formats such as `4.5 out of 5` into numerical values that could be analyzed in Excel.

Missing ratings were retained as missing.

### 4. Discount Cleaning

Discount values were converted from text percentages into numerical percentage values for calculations and categorization.

### 5. Price Cleaning

Currency text was removed from price values so that prices could be analyzed numerically.

One product contained a price range rather than a single price. The midpoint of the range was used for numerical analysis.

## Data Enrichment

Additional fields were created to improve the analysis:

* Discount Amount
* Rating Category
* Discount Category
* Price Category

The Discount Amount was calculated as:

```text
Old Price - Current Price
```

Rating and discount categories were also created using the thresholds specified in the project requirements.

## Excel Techniques Used

The project used several Excel features and techniques, including:

* Data cleaning
* Excel formulas
* Calculated columns
* Sorting and filtering
* Conditional formatting
* Pivot Tables
* Pivot Charts
* KPI calculations
* Correlation analysis
* Data categorization
* Dashboard design
* Slicers

## Descriptive Analysis

Key results from the cleaned dataset include:

| Metric                |       Result |
| --------------------- | -----------: |
| Total Products        |          112 |
| Average Current Price | KSh 1,186.89 |
| Average Old Price     | KSh 1,811.11 |
| Average Discount      |       36.78% |
| Average Rating        |     3.89 / 5 |
| Total Reviews         |          723 |
| Highest Current Price |    KSh 3,750 |
| Lowest Current Price  |       KSh 38 |

## Key Findings

### Discounts and Customer Engagement

The correlation between discount percentage and review count was approximately **-0.14**.

This is a very weak negative relationship, indicating that larger discounts did not necessarily generate more customer engagement.

### Price and Ratings

The correlation between current price and rating was approximately **+0.11**.

This is a very weak positive relationship, suggesting that higher-priced products were not necessarily rated substantially better.

### Ratings and Reviews

The relationship between ratings and review counts was approximately **+0.06**, indicating almost no linear relationship.

This means that products with many reviews were not automatically the products with the highest ratings.

### High-Performing Products

Products combining high review counts with strong ratings included:

* 137 Pieces Cake Decorating Tool Set
* Electronic Digital Display Vernier Caliper
* 3D Waterproof EVA Plastic Shower Curtain
* 100 Pcs Crochet Hook Tool Set
* Portable Mini Cordless Car Vacuum Cleaner

### Products Requiring Attention

Some products had high discounts but poor ratings. Examples include:

* 5-PCS Stainless Steel Cooking Pot Set
* 120W Cordless Vacuum Cleaner
* Intelligent LED Body Sensor Wireless Lighting Night Light
* 380ML USB Rechargeable Portable Small Blender
* Agapeon Toothbrush Holder and Toothpaste Dispenser

These products may require quality, pricing or customer-experience improvements rather than simply larger discounts.

## Business Recommendations

Based on the analysis, Jumia sellers should:

1. Avoid relying solely on large discounts to generate engagement.
2. Focus on product quality and customer satisfaction.
3. Monitor review counts together with ratings.
4. Investigate products with many reviews but low ratings.
5. Prioritize products with both high ratings and strong customer engagement.
6. Review heavily discounted products with poor customer ratings.
7. Maintain competitive prices while ensuring good product value.
8. Improve product descriptions, images and specifications to manage customer expectations.

## Dashboard

The Excel dashboard provides an interactive summary of product performance.

The dashboard includes:

* Total Products
* Average Current Price
* Average Discount
* Average Rating
* Total Reviews
* Top Products by Rating
* Top Products by Reviews
* Top Products by Discount
* Discount Category Analysis
* Rating Category Analysis
* Price Analysis
* Trend/relationship visualizations
* Interactive slicers

## Project Structure

The Excel workbook contains sections for:

1. Raw Data
2. Data Dictionary
3. Cleaned Data
4. Analysis
5. Business Insights
6. Pivot Tables
7. Dashboard

## Conclusion

The analysis demonstrates that product performance cannot be explained by discount percentage or price alone.

The strongest products tend to combine customer engagement with good ratings, while some highly reviewed or heavily discounted products still have poor ratings.

For sellers, the most effective strategy is therefore to balance competitive pricing and promotions with product quality, accurate product information and customer satisfaction.

## Tools Used

* Microsoft Excel
* Excel Power Query
* Pivot Tables
* Pivot Charts
* Excel formulas
* GitHub
* Markdown

## Author

This project was completed as part of an e-commerce data analysis project focused on Jumia product performance.
