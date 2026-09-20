# 🚗 Car Sales Analysis Dashboard – Power BI

## 📊 Project Overview

This project is an interactive **Car Sales Analysis Dashboard** created using **Microsoft Power BI**.

The dashboard analyzes car sales data and provides insights into sales performance, average selling prices, year-to-date (YTD) sales, month-to-date (MTD) sales, weekly sales trends, dealer regions, and individual car sales records.

The main objective of this project is to transform raw car sales data into meaningful and interactive business insights using Power BI and DAX.

---

## 📁 Dataset Information

The dataset is provided in an Excel file named:

**Car_Sales.xlsx**

### Dataset Size

- **Rows:** 23,906
- **Columns:** 16
- **Table Name:** `car_data`
- **Data Period:** 2022
- **File Format:** Microsoft Excel (`.xlsx`)

Each row represents a car sales record.

### Dataset Columns

| Column | Description |
|---|---|
| Car_id | Unique identifier for the car sale |
| Date | Date of the car sale |
| Customer Name | Name of the customer |
| Gender | Customer gender |
| Annual Income | Annual income of the customer |
| Dealer_Name | Name of the dealer |
| Company | Car manufacturer/company |
| Model | Car model |
| Engine | Engine type |
| Transmission | Transmission type |
| Color | Color of the car |
| Price ($) | Selling price of the car |
| Dealer_No | Dealer identification number |
| Body Style | Body style of the car |
| Phone | Customer phone number |
| Dealer_Region | Region where the dealer is located |

---

## 🛠️ Tools & Technologies

- **Microsoft Power BI**
- **Power Query**
- **DAX**
- **Microsoft Excel**

---

## 📌 Key KPIs

The dashboard contains the following key performance indicators:

### 💰 YTD Total Sales

Calculates the total sales amount from the beginning of the year up to the selected date.

### 💵 MTD Total Sales

Calculates the total sales generated during the current month up to the selected date.

### 📊 YTD Average Sale Price

Displays the average selling price of cars sold during the year up to the selected date.

### 💵 MTD Average Sale Price

Displays the average selling price of cars sold during the current month.

### 📈 YOY Growth %

Compares the current year's sales performance with the corresponding period of the previous year.

### 🔄 Previous Year Sales

Displays sales from the corresponding period of the previous year for comparison.

---

## 📈 Dashboard Visualizations

### 1. YTD Sales Weekly Trend

A line chart displays the weekly trend of Year-to-Date sales.

**X-axis:** Week Number  
**Y-axis:** YTD Total Sales

This visualization helps analyze how sales change throughout the year.

---

### 2. Cars Sold by Dealer Region

A map visualization displays car sales across different dealer regions.

Dealer regions are used as geographical locations, while the number of cars sold is used to represent sales volume.

This helps analyze the geographical distribution of car sales.

---

### 3. Detailed Car Sales Grid

A detailed table provides transaction-level information about individual car sales.

The table includes information such as:

- Car ID
- Model
- Body Style
- Color
- Sales Amount
- Dealer Name
- Dealer Region
- Date
- Company
- Engine
- Transmission
- Gender

---

## 📊 DAX Measures

The dashboard uses DAX measures for sales calculations and time-based analysis.

### Total Sales

```DAX
Total Sales =
SUM(car_data[Price ($)])
