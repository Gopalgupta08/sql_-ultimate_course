/* ==============================================================================
   SQL SELECT Query
-------------------------------------------------------------------------------
   This guide covers various SELECT query techniques used for retrieving, 
   filtering, sorting, and aggregating data efficiently.

   Table of Contents:
     1. SELECT ALL COLUMNS
     2. SELECT SPECIFIC COLUMNS
     3. WHERE CLAUSE
     4. ORDER BY
     5. GROUP BY
     6. HAVING
     7. DISTINCT
     8. TOP
     9. Combining Queries
	 10. COOL STUFF - Additional SQL Features
=================================================================================
*/
use master;

-- Retrive all Customers Data
SELECT *FROM customers;

-- Retrive all Oreder Data
SELECT * FROM orders;

-- Retrive each customer's name, country,and score.
SELECT
	first_name,
	country,
	score
FROM customers;

-- retrive customers with a score not equal to 0.
SELECT * FROM customers 
WHERE score != 0; 

-- Retrive customers from Germany
SELECT * FROM customers
WHERE country = 'Germany';

-- Retrive the name and country of customers from Germany
SELECT 
	first_name,
	country
FROM customers
WHERE country = 'Germany';

-- Retrieve all customers and sort the results by the highest score first.
SELECT * FROM customers
ORDER BY score DESC;

-- Retrieve all customers and sort the result by the lower score first.
SELECT * FROM customers
ORDER BY score ASC;

-- Retrieve all customers and sort results by the country.
SELECT * FROM customers ORDER BY country ASC;

-- Retrieve all customers and sort results by the country and then by the higehest score.
SELECT *FROM customers 
ORDER BY
	country ASC,
	score DESC

-- Retrieve thre name ,country , and score of customers whose score is not equal to 0 and sort results by the highest score first.
SELECT 
	first_name,
	country,
	score
FROM customers
WHERE score != 0
ORDER BY score DESC
