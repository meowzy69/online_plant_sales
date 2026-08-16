
# Online Plant Listings — Market & Pricing Analysis

An Excel analysis of the online plant retail market — web-scraped from e-commerce listings, cleaned with Power Query, and visualized in a fully interactive Excel dashboard to understand pricing, discounting, and product-mix patterns across brands, plant types, and sizes.

---

## Project Overview

Online plant sellers vary widely in pricing, discounting, and product range. This project scrapes and cleans real online plant listings, then builds an interactive Excel dashboard to understand how price, discount, plant type, size, and seller brand relate to one another — surfacing patterns useful for sellers, buyers, and market researchers.

---

## Project Objective

This project analyzes online plant listing data to answer key questions:

* Which brands/sellers list the most plants?
* How are plants distributed across types (Fruit, Flower, Herb, Bamboo, etc.)?
* What share of listings are considered feng shui–friendly?
* How are plants split across life cycle (Annual / Perennial / Biennial)?
* What plant sizes dominate the market?
* What is the average price and typical discount offered?

---

## Tools Used

* Microsoft Excel
* Power Query (data cleaning & transformation)
* PivotTables & PivotCharts
* Excel formulas (for KPI calculations)
* Web Scraper (Chrome extension) for data collection

---

## Dataset Information

Plant listings were scraped from an online marketplace, capturing fields such as:

* Plant Name & Brand
* Original Price & Special (Discounted) Price
* Discount Percentage
* Plant Size (Small / Medium / Large)
* Plant Type (Fruit, Flower, Herb, Bamboo, Foliage, Succulent, Bonsai, Shrub, etc.)
* Life Cycle (Annual / Perennial / Biennial)
* Feng Shui Suitability
* Hybrid Status
* Return Policy
* Location

**Raw dataset:** 440 scraped listings
**Cleaned dataset:** 400 listings after validation

---

## Data Cleaning & Transformation

Data preparation was performed entirely in Excel using Power Query:

* Removed scraper metadata columns not needed for analysis (start URL, pagination links)
* Standardized column names for consistency
* Corrected data types for price, discount, and size fields
* Removed duplicate and incomplete listings
* Validated categorical fields (type, life cycle, feng shui, hybrid status)
* Converted size labels into a consistent Small/Medium/Large scale
* Loaded the cleaned table into the workbook's data model for dashboard reporting

---

## Dashboard Features

Built natively in Excel using PivotTables, PivotCharts, and linked KPI cards.

### Executive KPIs

* Plant Count
* Average Price
* Average Discount

### Product Mix Analysis

* Plant Count by Brand
* Feng Shui Suitability Split
* Plant Count by Life Cycle
* Plant Size Distribution
* Return Policy Breakdown

---

## Key Insights

* The cleaned dataset covers **351 plant listings** (as shown on the dashboard) across **154 unique brands**, with **greenhousestore**, **UGAOO**, and **Cloud Farm** among the top listers.
* Average listed price is **₹144.18** (post-discount), with an **average discount of 66%** off the original price — discounting is the norm rather than the exception in this market.
* **Fruit** and **Flower** plants are the two largest categories by listing count, followed by **Herb** and **Bamboo**.
* Life cycle is split fairly evenly between **Annual (~50%)** and **Perennial (~45%)** plants, with **Biennial** plants a small minority.
* **56% of listings are not marketed as feng shui–friendly**, while 44% are.
* **Small-sized plants dominate the market (74%)**, followed by Medium (26%); Large plants are rare.
* **100% of listings in this dataset offer no returns**, indicating a market-wide no-returns norm for plant purchases.

---

## Repository Structure

```text
online_plant_listings
│
├── Clean_data
│   └── Cleaned_data.csv.xlsx
│
├── Raw_data
│   └── plant_url.xlsx
│
├── Reports
│   └── Online_plant_listings_dashboard.xlsx
│
└── README.md
```

---

## Future Improvements

* Expand scraping to additional marketplaces for cross-platform price comparison
* Track price and discount trends over time
* Add brand-level rating/quality correlation analysis
* Build a recommendation view for best-value plants by type and size
* Automate periodic re-scraping and dashboard refresh using Power Query

---

## Author

**Chandrapal Solanki**
Aspiring Data Analyst with interests in Excel, Power BI, SQL, and data visualization. Focused on transforming raw data into actionable business insights.
