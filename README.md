# AdventureWorks-using-Azure-SQL
# ☁️ Explore Relational Data in Azure SQL

This project demonstrates how to explore and query relational data using **Azure SQL Database** with the **AdventureWorks** sample dataset. It showcases the use of Azure's built-in query editor to interact with structured data in a cloud-hosted SQL environment.

---

## 📌 About the Project

The goal of this project is to provide hands-on experience with:
- Connecting to an Azure SQL Database
- Exploring relational tables and schemas
- Writing and executing SQL queries in the Azure portal
- Understanding how cloud-based relational databases work

---

## 🧱 Database Details

- **Database Name**: `AdventureWorks`
- **Server Name**: `sqlserver52093791`
- **Schema Examples**:
  - `dbo.BuildVersion`
  - `dbo.ErrorLog`
  - `SalesLT.Address`
  - `SalesLT.Customer`
  - `SalesLT.Product`

---

## 🧪 Sample Query


SELECT * FROM SalesLT.Product;

![azure 3](https://github.com/user-attachments/assets/a8475634-eec9-455a-9bea-75853247894d)


SELECT ProductID, Name, ListPrice, ProductCategoryIDFROM SalesLT.Product;

![azure 2](https://github.com/user-attachments/assets/84f16bc2-9290-4ef4-b6cb-92c1dbf148d4)


SELECT p.ProductID, p.Name AS ProductName,       c.Name AS Category, p.ListPriceFROM SalesLT.Product AS pJOIN [SalesLT].[ProductCategory] AS c   ON p.ProductCategoryID = c.ProductCategoryID;

![azure](https://github.com/user-attachments/assets/fcc74443-8b36-47b7-afce-87ceef51a630)
