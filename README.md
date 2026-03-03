# Book Subcategory Analytics Dashboard - Power BI

![Status](https://img.shields.io/badge/Status-Completed-brightgreen)
![Version](https://img.shields.io/badge/Version-v2.0-blue)
![Data](https://img.shields.io/badge/Data-999%20Books-orange)
![Tool](https://img.shields.io/badge/Tool-PowerBI-yellow)

---

## Overview
Interactive and visually rich Power BI dashboard built on scraped book data with extended **subcategory analytics**.

Enables stakeholders to explore pricing trends, availability patterns, rating distribution, and outliers across subcategories like Travel, Music, Science, Fiction, and more.

---

## Data Modeling & Processing
- Added **Subcategory** field (derived from category URLs)
- Converted **GBP (£) → USD ($)** using £1 = $1.32
- Implemented Price Categories:
  - **Budget:** < $30.00
  - **Standard:** $30.00 - $60.00
  - **Premium:** > $60.00
- Cleaned data in Power Query (removed duplicates, trimmed spaces, handled nulls)
- Enforced correct data types (Price → Decimal, Rating → Whole Number)

---

## Visualizations Implemented
- **Tree Map** – Book count & average price by subcategory  
- **Decomposition Tree** – Category → Subcategory → Rating → Availability → Price Tier  
- **KPI Cards/Grid** – Total Books, Avg Price, % In Stock, Highest Rated Book  
- **Stacked Column Chart** – Availability by Subcategory  
- **Scatter Plot + Trend Line** – Price vs Rating (colored by subcategory)  
- **Smart Narrative** – Auto-generated insights  
- **Bookmarks Navigation** – Overview | Pricing | Availability | Deep Dive  

---

## Interactive Filters
- Subcategory  
- Rating (1–5)  
- Price Category  
- Availability  

All visuals update dynamically.

---

## Key Findings
- Majority of books fall under the **Standard price tier** (~$46 average).
- Weak positive correlation between **price and rating**.
- Some high-rated books are **out of stock**, indicating demand gaps.
- Inventory is concentrated in a few dominant subcategories.
- Niche subcategories show potential for premium pricing.

---

## Project Structure
project/
│── powerbi/
│ ├── Book_Subcategory_Analytics_Dashboard.pbix
│── scraper.py
│── books_data_extended.csv
│── README.md

---

## Status
✔ Subcategory integration completed  
✔ USD conversion applied  
✔ Price tier classification implemented  
✔ Advanced visuals with drill & regression  
✔ Bookmark navigation enabled  

---

### Outcome
A fully interactive decision-support dashboard for pricing strategy, inventory optimization, and subcategory performance analysis.
