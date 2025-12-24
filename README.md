# Customer-Behavior-Analysis-Using-SQL-A-Case-Study-of-Danny-s-Diner
SQL analysis of Danny’s Diner – 8 Week SQL Challenge (Week 1)

INTRODUCTION
The 8 Week SQL Challenge is a collection of real-world inspired SQL case studies created to help analysts strengthen their SQL and analytical thinking skills. Each case study focuses on answering business questions using available data.

In this project, I walk through my solution to Week 1: Danny’s Diner, where I used SQL to analyze customer purchasing behavior for a small restaurant. The goal of this project is not just to write SQL queries, but to derive meaningful business insights that can help improve decision-making.

This project demonstrates my ability to:

Understand business problems
Work with relational datasets
Write clean and efficient SQL queries
Translate results into actionable insights
Business Problem
Danny recently opened a small restaurant called Danny’s Diner that serves a limited menu of dishes. While the restaurant has been operating for a short time, Danny wants to better understand his customers in order to:

Identify top-spending customers
Understand which menu items are most popular
Evaluate the impact of his customer loyalty program
By analyzing customer, sales and membership data, we can help Danny make informed decisions about promotions, menu design, and customer retention strategies.

Dataset Description
The analysis is based on three tables, all sourced from https://8weeksqlchallenge.com/case-study-1/ :

1. sales
This table records every purchase made by customers and it contains 3 columns.

customer_id
order_date
product_id
2. menu
This table contains information about menu items i.e the products being sold and it contains 3 columns.

product_id
product_name
price
3. members
This table tracks when customers joined danny’s loyalty program and it contains 2 columns.

customer_id
join_date
The sales and menu tables are linked through product_id, the sales table is also linked to members table through customer_id. This allows us to combine purchase behavior with pricing and membership information.

Tool Used
Microsoft SQL Server

OBJECTIVES
The key objectives of this analysis are:

To identify high value customers based on total spending
To understand how frequent the customers visit the restaurant
To understand customer’s initial preferences
To identify the restaurant’s best selling product
To analyze customer’s favorite item on the menu
To evaluate whether membership influences purchasing behavior
Business Questions
Using SQL, I answered the following business questions

What is the total amount each customer spent at the restaurant?
How many days has each customer visited the restaurant?
What was the first item from the menu purchased by each customer?
What is the most purchased item on the menu and how many times was it purchased by all customers?
Which item was the most popular for each customer?
Which item was purchased first by the customer after they became a member?
Which item was purchased just before the customer became a member?
What is the total items and amount spent for each member before they became a member?
If each $1 spent equates to 10 points and sushi has a 2x points multiplier — how many points would each customer have?
In the first week after a customer joins the program (including their join date) they earn 2x points on all items, not just sushi — how many points do customer A and B have at the end of January?
