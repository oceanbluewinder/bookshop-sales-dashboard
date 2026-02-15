# bookshop-sales-dashboard

Power BI dashboard analyzing bookstore sales data from MySQL.

---

## Project Overview

This project demonstrates a complete end-to-end data analysis workflow:

- Data stored in MySQL
- Data modeling in Power BI
- KPI calculation using DAX
- Dashboard visualization
- Publishing project to GitHub

The purpose of this project is to practice applying learned skills into a complete workflow, from data preparation to visualization and final GitHub publishing.

This project focuses on sales analysis and dashboard design rather than predictive modeling.

---

## Data Source

- Database: MySQL
- Database Name: bookshop
- Tables Used:
  - book
  - customer
  - publisher
  - order_master
  - order_detail
  - purchase

---

## Data Model

The database follows a relational structure:

- order_master links to customer
- order_detail links to order_master and book
- book links to publisher

ERD is available in the `erd/` folder.

---

## Key Metrics

### Total Revenue
Sum of quantity multiplied by book price for all order records.

Formula:
Total Revenue = SUM ( quantity × price )

---

### Order Count
Number of distinct order_id.

Formula:
Order Count = DISTINCTCOUNT ( order_id )

---

### Average Order Value
Total revenue divided by number of orders.

Formula:
Average Order Value = Total Revenue / Order Count

---

### Best Selling Books
Books ranked by total quantity sold.

Formula:
Total Quantity Sold = SUM ( quantity )

---

## Dashboard Features

- KPI Cards
  - Total Revenue
  - Order Count
  - Average Order Value
- Monthly Revenue Trend
- Top 5 Best-Selling Books
- Clean layout suitable for business reporting

Dashboard screenshot is available in the `screenshots/` folder.

---

## Purpose of This Project

This project is a practical learning exercise.

The goal was to:
- Apply SQL and data modeling knowledge
- Practice Power BI visualization
- Complete the full workflow from database to GitHub
- Build a portfolio-ready project

---

## Tools Used

- MySQL
- Power BI Desktop
- GitHub
- dbdiagram.io

---

## Author

OceanBlueWinder
