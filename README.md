# Coffee Shop Sales Insights

A comprehensive data analysis project that leverages Microsoft Excel to analyze coffee shop sales data, providing actionable business insights through data cleaning, exploratory data analysis, and interactive visualizations.

## 📊 Project Overview

This project analyzes comprehensive coffee shop transaction data containing 149,116 records across multiple store locations. The dataset includes detailed transaction information with timestamps, product details, store locations, and customer purchase patterns. Using Excel's analytical capabilities, I transformed this transactional data into actionable business insights.

## 🎯 Objective

- Analyze sales performance and identify revenue growth opportunities
- Understand customer purchasing patterns and preferences
- Evaluate product performance and seasonal trends
- Create actionable insights for business optimization
- Develop an interactive dashboard for ongoing sales monitoring

## 🧹 Data Cleaning Process

### Dataset Structure:
- **Transaction Data**: 149,116+ records with unique transaction IDs
- **Store Information**: Multiple locations (Astoria, Hell's Kitchen, Lower Manhattan)
- **Product Details**: Categories (Coffee, Tea, Bakery, etc.) with specific product types and sizes
- **Time Analysis**: Date, time, hour, day of week, and month columns for temporal analysis
- **Financial Data**: Unit prices, quantities, and total bill calculations

### Data Quality Issues Addressed:
- **Date/Time Formatting**: Standardized transaction_date and transaction_time formats
- **Derived Columns**: Created Day Name, Month Name, Hour, Day of Week for analysis
- **Price Calculations**: Verified unit_price × transaction_qty = Total_bill consistency
- **Product Categorization**: Ensured proper product_category, product_type, and product_detail alignment
- **Store Location Validation**: Verified store_id matches with store_location data

### Excel Functions Used:
- `TRIM()`, `CLEAN()` for text cleaning
- `IFERROR()`, `ISBLANK()` for handling missing data
- Conditional formatting for data quality checks
- Data validation rules for consistency

## 🔍 Exploratory Data Analysis (EDA)

### Sales Performance Analysis:
- **Hourly Trends**: Peak sales hours (11 AM - 2 PM based on sample data)
- **Daily Patterns**: Weekend vs weekday performance analysis
- **Monthly Trends**: June sales patterns and seasonal variations
- **Store Comparison**: Performance across Astoria, Hell's Kitchen, and Lower Manhattan

### Product Analysis:
- **Category Performance**: Coffee, Tea, Bakery, and other product categories
- **Product Types**: Brewed herbal tea, espresso drinks, pastries analysis
- **Size Preferences**: Large, Medium, Small size distribution
- **Price Points**: Unit price analysis across different product categories

### Location Insights:
- **Store Performance**: Revenue comparison across 3+ store locations
- **Geographic Trends**: Location-based product preferences
- **Operational Hours**: Peak times by store location
- **Product Mix**: Category distribution by store

## 📈 Key Metrics & Calculations

### Revenue Metrics:
- **Total Revenue**: `=SUMPRODUCT(transaction_qty, unit_price)`
- **Average Transaction Value**: `=AVERAGE(Total_bill)`
- **Daily Sales**: `=SUMIFS(Total_bill, transaction_date, criteria)`
- **Hourly Revenue**: `=SUMIFS(Total_bill, Hour, hour_criteria)`

### Performance Indicators:
- **Top Products**: `=RANK(SUMIFS(Total_bill, product_detail, product), revenue_range)`
- **Store Performance**: `=SUMIFS(Total_bill, store_location, location)`
- **Category Analysis**: `=SUMIFS(Total_bill, product_category, category)`
- **Time-based Trends**: `=SUMIFS(Total_bill, Day_Name, day)` and `=SUMIFS(Total_bill, Month_Name, month)`

### Advanced Calculations:
- **Peak Hour Analysis**: `=MAXIFS(Total_bill, Hour, hour_range)`
- **Day of Week Performance**: `=SUMIFS(Total_bill, Day_of_Week, weekday_number)`
- **Product Mix by Store**: `=COUNTIFS(store_location, location, product_category, category)`
- **Average Transaction by Time**: `=AVERAGEIFS(Total_bill, Hour, time_criteria)`

## 🛠️ Tools Used

### Excel Functions & Formulas:
- **Lookup Functions**: `VLOOKUP()`, `INDEX()`, `MATCH()`
- **Statistical Functions**: `AVERAGE()`, `MEDIAN()`, `STDEV()`
- **Date Functions**: `YEAR()`, `MONTH()`, `WEEKDAY()`
- **Conditional Functions**: `SUMIFS()`, `COUNTIFS()`, `AVERAGEIFS()`

### Data Analysis Features:
- **Pivot Tables**: Dynamic data summarization and cross-tabulation
- **Pivot Charts**: Interactive visualizations linked to pivot tables
- **Data Tables**: Scenario analysis and sensitivity testing
- **Conditional Formatting**: Visual data highlighting and trend identification

### Visualization Tools:
- **Charts**: Column, line, pie, and combination charts
- **Sparklines**: Micro-charts for trend visualization
- **Slicers**: Interactive filtering for dashboards
- **Timeline Controls**: Date-based filtering capabilities

## 💡 Key Insights & Results

### Sales Performance:
- **Peak Hours**: 11 AM - 2 PM show highest transaction volumes
- **Weekend Performance**: Saturday and Sunday demonstrate strong sales patterns
- **Store Distribution**: Astoria location shows consistent performance across different hours
- **Average Transaction**: $3.00 for tea products with consistent pricing

### Product Insights:
- **Tea Category**: Brewed herbal tea (Peppermint) shows regular customer demand
- **Size Preference**: Large size products demonstrate customer preference
- **Product Consistency**: Uniform pricing across same product types
- **Category Distribution**: Tea, Coffee, and Bakery items across multiple locations

### Operational Insights:
- **Store Coverage**: 3+ locations (Astoria, Hell's Kitchen, Lower Manhattan)
- **Operating Hours**: Extended hours from morning (11 AM) to evening (7 PM)
- **Product Availability**: Consistent product offerings across locations
- **Transaction Patterns**: Regular customer visits throughout weekdays and weekends

### Business Recommendations:
- Optimize inventory for high-performing products during peak seasons
- Implement targeted promotions for underperforming time periods
- Focus marketing efforts on customer retention strategies
- Expand successful product categories based on profitability analysis

## 📊 Dashboard Features

- **Store Performance**: Revenue comparison across Astoria, Hell's Kitchen, and Lower Manhattan
- **Time Analysis**: Hourly, daily, and monthly sales trend visualizations
- **Product Categories**: Interactive filtering by Coffee, Tea, Bakery categories
- **Peak Hours**: Visual identification of high-traffic time periods
- **Location Insights**: Geographic performance and product mix analysis

## 🎯 Conclusion

This Excel-based analysis successfully transformed raw coffee shop sales data into actionable business insights. The comprehensive dashboard and detailed metrics provide stakeholders with the tools needed to make data-driven decisions for revenue optimization and customer satisfaction improvement.

The project demonstrates the power of Excel's analytical capabilities in delivering professional-grade business intelligence solutions without requiring specialized software or programming knowledge.

---

**Technologies Used**: Microsoft Excel | **Analysis Type**: Sales Analytics | **Industry**: Food & Beverage

**Key Skills Demonstrated**: Data Cleaning, Statistical Analysis, Data Visualization, Business Intelligence, Dashboard Development