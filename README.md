## MOBILE-SALES-ANALYSIS

## OVERVIEW:
+ This is a sales report for a Mobile Product

    ---

## Project Overview:
+ This project analysis the sales of mobile sales product to uncover insights such as customers,gender and payment,using Pivot tables,I explored metrics like Total sales by payment method and Gender,Average income of buyers,gender distribution,and overrall revenue.

---

## Contents:
Projects overview|Data Source|Tools Used|Table Outlay|Query Languages(SQL)|Visualization

---
## Data Source:
www.kagggle.com/dataset

---

## Tools Used:
+ Pivot Table/Chart
+ PowerBI
+ SQL

  ---

## Table Outlay:
First three Records
|TransactionID|	Date| MobileModel|	Brand|	Price|	UnitsSold|	TotalRevenue|	CustomerAge	|CustomerGender|	Location|	PaymentMethod|
|------|-----|----|-------|-------|----------|--------|--------|------|-------|---------|
|79397f68-61ed-4ea8-bcb2-f918d4e6c05b|	1/6/2024|	direction|	Green Inc|	1196.95|	85|	28002.8|	32|	Female|	Port Erik|	Online|
|4f87d114-f522-4ead-93e3-f336402df6aa|	4/5/2024|	right|	Thomas-Thompson	|1010.34|	64|	2378.82|	55|	Female|	East Linda|	Credit Card||
|6750b7d6-dcc5-48c5-a76a-b6fc9d540fe1|	2/13/2024|	summer|	Sanchez-Williams|	400.8|	95|	31322.56|	57|	Male|	East Angelicastad|	Online|

---

## Query Languages(SQL):
Some of the query language used to retrieve records are displayed here:
````SQL
 SELECT * FROM 'mobile sales';
---Calculate Total Revenue By Price---
SELECT Paymentmethod,Sum(price)
AS Total Revenue
FROM mobile sales
GROUP BY Payment
ORDER BY Total Revenue DESC;

````SQL
SELECT* FROM 'mobile sales';
--- Categorise data into silver,gold,and daimond---
CASE
WHEN price <500 THEN 'Silver'
WHEN price BETWEEN 500 AND 1000 THEN 'Gold'
ELSE 'Diamond'
ENS AS Category
FROM mobile sales;

---

## Visualization

## Pivot Tables



  

