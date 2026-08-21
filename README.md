# Zomato SQL Project

## 📌 Project Overview
This project is a comprehensive SQL-based system inspired by Zomato's operations. It demonstrates how to create, manage, and analyze a relational database for a restaurant management system. The project includes essential tables for restaurants, customers, orders, and reviews, along with insightful queries for data analysis.

## 📂 Features
- **Database Structure:** Tables for restaurants, customers, orders, and reviews.
- **Data Insertion:** Sample data for realistic scenarios.
- **Advanced Queries:** Analysis of:
  - Top-performing restaurants.
  - Customer behavior patterns.
  - Revenue trends.
- **Optimization:** Demonstrates SQL best practices for efficiency and scalability.

## 🔧 Technologies Used
- **Database:** SQL Server
- **Language:** SQL
- **Tools:** SQL Server Management Studio (SSMS)

## 🚀 Getting Started

### Prerequisites
- SQL Server installed on your system.
- SQL Server Management Studio (SSMS) for database management.

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/Beware2707/Zomato-SQL-Project.git
   ```
2. Open `ZOMATO SQL PROJECT.sql` in SSMS.
3. Execute the script to create and populate the database tables, then run the analysis queries to generate insights.

## 📊 Sample Queries

Identify the top 5 restaurants by revenue:
```sql
SELECT TOP 5 RestaurantName, SUM(OrderAmount) AS TotalRevenue
FROM Orders
GROUP BY RestaurantName
ORDER BY TotalRevenue DESC;
```

Analyze customer behavior:
```sql
SELECT CustomerID, COUNT(OrderID) AS TotalOrders
FROM Orders
GROUP BY CustomerID
ORDER BY TotalOrders DESC;
```

## 🌟 Insights
- Restaurants with the highest revenue.
- Peak ordering times and days.
- Customer preferences and feedback trends.

## 📧 Contact
For questions or suggestions, feel free to reach out:

- **Name:** Jai Pratap Singh
- **Email:** riddlesforeverbiz@gmail.com
- **GitHub:** [Beware2707](https://github.com/Beware2707)
