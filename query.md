SQL database dump is in db_dump.sql file above. Download `db_dump.sql` file to your local computer.

###  Data Analysis Using SQL (Queries )

1. Query to show all customer records

      `SELECT * FROM sales.customers;`

2. Query to show total number of customers

    `SELECT COUNT(*) FROM sales.customers;`
3. Query to show all the date records

   `SELECT * FROM sales.date;`
4. Query to show all the market records

   `SELECT * FROM sales.markets;`
5. Query to show total number of markets 

   `SELECT COUNT(*) FROM sales.markets;`
6. Query to show all the product records

   `SELECT * FROM sales.products;`
7. Query to show total number of productc 

   `SELECT COUNT(*) FROM sales.products;`
8. Query to show all the transaction records

   `SELECT * FROM sales.transactions;`
9. Query to show total number of transactions

   `SELECT COUNT(*) FROM sales.transactions;`
   
10. Query to show total sales 

    `SELECT SUM(sales_amount) FROM sales.transactions;`
   
11. Query to show total sales based on year

    `SELECT distinct YEAR (order_date) , SUM(sales_amount) FROM sales.transactions GROUP BY YEAR(order_date);`

12. Query to show distinct customer type 

     `SELECT DISTINCT customer_type FROM sales.customers;`

13. Query to show various market name

    `SELECT DISTINCT markets_name FROM sales.markets;`
   
14. Query to show various market zones

    `SELECT DISTINCT zone FROM sales.markets;`

15. Query to show various product types

    `SELECT DISTINCT product_type FROM sales.products;`
   
16. Query to show first 5 transaction records

    `SELECT * FROM sales.transactions LIMIT 5;`
   
17. Query to show sales transactions which is in US dollars

    `SELECT * FROM sales.transactions WHERE currency = "USD";`
   
18. Query to show transactions for Chennai market (market code for chennai is Mark001)

    `SELECT * FROM sales.transactions WHERE market_code='Mark001';`

19. Query to show distrinct product codes that were sold in chennai

    `SELECT DISTINCT product_code FROM transactions WHERE market_code='Mark001';`

20. Query to show all the transactions where currency is US dollars

    `SELECT * from transactions where currency="USD";`
