# 📚 Online Bookstore Database Management & Analysis

## 📌 Project Overview
This project focuses on designing and querying a relational database for an online bookstore using PostgreSQL. It organizes information about books, customers, and orders and provides a foundation for analyzing sales, inventory, and customer purchasing behavior.

## 🛠️ Technologies Used
- PostgreSQL
- SQL
- Visual Studio Code
- SQLTools Extension

## 🗄️ Database Structure
The database consists of three tables:

### 1. Books
Stores information about books.
- `Book_ID` — Primary key
- `Title` — Book title
- `Author` — Author name
- `Genre` — Book genre
- `Published_Year` — Year of publication
- `Price` — Book price
- `Stock` — Available stock

### 2. Customers
Stores customer information.
- `Customer_ID` — Primary key
- `Name` — Customer name
- `Email` — Email address
- `Phone` — Contact number
- `City` — Customer city
- `Country` — Customer country

### 3. Orders
Stores bookstore order details.
- `Order_ID` — Primary key
- `Customer_ID` — Foreign key referencing `Customers`
- `Book_ID` — Foreign key referencing `Books`
- `Order_Date` — Date of order
- `Quantity` — Quantity ordered
- `Total_Amount` — Total order amount

## 🔗 Database Relationships
- One customer can place multiple orders.
- One book can appear in multiple orders.
- The `Orders` table connects customers and books using foreign keys.

## 📊 SQL Tasks Covered

### Basic Queries
1. Retrieve books in the Fiction genre.
2. Find books published after 1950.
3. List customers from Canada.
4. Retrieve orders placed in November 2023.
5. Calculate the total stock of books.
6. Find the most expensive book.
7. Identify customers who ordered more than one book in an order.
8. Retrieve orders with a total amount above $20.
9. List available book genres.
10. Find the book with the lowest stock.
11. Calculate total revenue from orders.

### Advanced Queries
1. Calculate books sold by genre.
2. Find the average price of Fantasy books.
3. Identify customers who placed at least two orders.
4. Find the most frequently ordered book.
5. Retrieve the three most expensive Fantasy books.
6. Calculate quantities sold by each author.
7. Find cities of customers who spent more than $30.
8. Identify the customer who spent the most.
9. Calculate remaining stock after fulfilling orders.

## 💡 SQL Concepts Covered

- DDL (Data Definition Language): `CREATE TABLE`, `DROP TABLE`
- Data Retrieval: `SELECT`, `WHERE`, `DISTINCT`, `ORDER BY`, `LIMIT`
- Aggregate Functions: `COUNT()`, `SUM()`, `AVG()`, `MIN()`, `MAX()`
- Grouping and Filtering: `GROUP BY`, `HAVING`
- Joins: `INNER JOIN`, `LEFT JOIN` to combine books, customers, and order data
- Subqueries: To answer advanced analytical questions
- Constraints: Primary keys, foreign keys, and `SERIAL`
- Business Analysis: Sales revenue, customer spending, genre-wise sales, and inventory management

## 🎯 Learning Outcomes
- Creating relational tables with primary and foreign keys.
- Retrieving and filtering records using `SELECT` and `WHERE`.
- Sorting and limiting query results.
- Applying aggregate functions such as `SUM`, `AVG`, and `COUNT`.
- Analyzing customer orders, book sales, revenue, and inventory.

## ▶️ How to Run
1. Install PostgreSQL and VS Code.
2. Connect to PostgreSQL using the SQLTools extension.
3. Create or select the target database.
4. Open `onlinebookstore.sql` in VS Code.
5. Execute the table creation statements.
6. Insert or import sample data into the tables.
7. Run the analysis queries and inspect the results.

## 📁 Project Files
- `onlinebookstore.sql` — Table creation and SQL practice queries.
- `README.md` — Project documentation.
- `screenshots/` — Query output screenshots.

## 👤 Author
Tanmay More

---

*This project was created for SQL practice and to develop practical database querying and data analysis skills.*