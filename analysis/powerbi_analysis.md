# Power BI Mobile Sales Dashboard — Technical + Business Analysis

This document provides a complete analysis of the Mobile Sales Dashboard built in Power BI.  
It covers both **business insights** and **technical implementation**

---

# 1. Dataset Overview (Based on Data Pane)

The dataset contains the following key fields:

### **Dimensions**

- Brand
- City
- Customer Name
- Customer Age
- Customer Rating
- Date
  - Day Name
  - Month
  - Year
- Mobile Model
- Payment Method

### **Measures / Numeric Fields**

- Total Sales
- Total Quantity
- Total Transactions
- Price Per Unit
- Average (calculated)

These fields support multi‑dimensional analysis across **time, geography, product, customer behavior, and payment methods**.

---

# 2. Key Performance Indicators (KPIs)

The dashboard displays four primary KPIs:

### **1. Total Sales — 769M**

Overall revenue generated across all brands and models.

### **2. Total Quantity Sold — 19K**

Indicates product movement and demand.

### **3. Total Transactions — 4K**

Shows customer purchase volume.

### **4. Average Sales — 40K**

Represents average revenue per transaction.

These KPIs form the foundation of performance evaluation.

---

# 3. Geographic Insights — Sales by City

The map visualization highlights:

- Highest sales in major metro cities (e.g., New Delhi, Mumbai)
- Strong presence across India, Nepal, Bangladesh, Sri Lanka
- Larger bubbles represent higher revenue contribution

### **Business Insight**

Urban regions drive the majority of sales, indicating:

- Higher purchasing power
- Strong brand presence
- Better retail penetration

---

# 4. Time‑Series Insights

## **A. Total Quantity by Month**

Monthly trend shows:

- Peaks in **March, June, December**
- Dips in **February, September**

### **Interpretation**

These patterns may be influenced by:

- Seasonal demand
- Festival periods
- Promotional campaigns

---

## **B. Total Sales by Day Name**

Daily trend shows:

- Highest sales on **Saturday, Monday, Friday**
- Lowest on **Wednesday**

### **Interpretation**

- Weekends show strong customer activity
- Mid‑week dips indicate lower footfall or online activity

---

# 5. Brand Performance Analysis

| Brand   | Total Sales | Quantity | Transactions |
| ------- | ----------- | -------- | ------------ |
| Apple   | 161M        | 3932     | 783          |
| Samsung | 160M        | 3923     | 775          |
| OnePlus | 153M        | 3830     | 768          |
| Vivo    | 150M        | 3801     | 766          |
| Xiaomi  | 143M        | 3664     | 743          |

### **Insights**

- Apple leads in revenue
- Samsung is extremely close, showing strong competition
- Xiaomi has lower revenue but strong volume
- All brands have similar transaction counts

### **Business Interpretation**

- Premium brands drive revenue
- Mid‑range brands drive volume
- Balanced product portfolio

---

# 6. Product Insights — Sales by Mobile Model

Top‑selling models:

- **iPhone SE — 60M**
- **OnePlus Nord — 58M**
- **Galaxy Note 20 — 56M**

### **Interpretation**

- Mid‑range and premium models dominate
- Strong customer preference for feature‑rich devices

---

# 7. Customer Ratings Analysis

- 5‑Star: 2K
- 4‑Star: 1K
- 3‑Star and below: Very low

### **Insight**

High customer satisfaction across brands and models.

---

# 8. Payment Method Insights

Pie chart shows:

- Debit Card — 26.2%
- UPI — 22.8%
- Other methods evenly distributed

### **Interpretation**

Digital payments dominate, indicating:

- Tech‑savvy customers
- Faster checkout experience
- Reduced cash dependency

---

# 9. Technical Implementation (Power BI)

## **A. Data Modeling**

- Single‑table model (flat structure)
- Ideal for dashboards with no relational complexity
- Supports fast filtering and slicer performance

## **B. Power Query**

Used for:

- Data type correction
- Column renaming
- Date hierarchy extraction (Day Name, Month, Year)
- Ensuring clean, analysis‑ready data

## **C. DAX Measures**

Examples:

- Total Sales = SUM(Mobile_sales_Data[Total Sales])
- Total Quantity = SUM(Mobile_sales_Data[Total Quantity])
- Total Transactions = SUM(Mobile_sales_Data[Total Transactions])
- Average Sales = DIVIDE([Total Sales], [Total Transactions])

These measures power the KPI cards and visuals.

## **D. Visuals Used**

- Map
- Line charts
- Bar charts
- Pie chart
- Table
- KPI cards
- Slicers

Each visual is chosen to match the data type and insight requirement.

---

# 10. Business Recommendations

- Increase stock for high‑selling models
- Run weekend promotional campaigns
- Improve mid‑week engagement
- Expand presence in high‑potential cities
- Promote UPI/EMI offers to boost conversions
- Focus on premium models for higher revenue

---

# Author

**Vishal Thakare**  
Power BI | Data Analytics | Business Intelligence
