# SQL_Lab_One

1. SELECT * FROM Customers

2. SELECT DISTINCT country FROM customers;

3. SELECT * FROM customers WHERE customerid LIKE 'BL%';

4. SELECT * FROM orders LIMIT 100;

5. SELECT * FROM customers WHERE postalcode IN ('1010', '3012', '12209', '05023');

6. SELECT * FROM orders WHERE shipregion IS NOT NULL;

7. SELECT * FROM customers ORDER BY country, city;

8. INSERT INTO customers ( customerid, companyname, contactname, contacttitle, address, city, region, postalcode, country, phone, fax )
values ('MARK', 'Stark Industries', 'Tony Stark', 'Iron man', 'Stark Towers', 'New York', 'HHHH', '99999', 'USA', '1801801808', '8786-8765' );

9. UPDATE orders SET shipregion='EuroZone' WHERE shipcountry='France';

10. DELETE FROM order_details WHERE quantity = '1';

11. SELECT AVG(quantity) FROM order_details;
	SELECT MAX(quantity) FROM order_details;
	SELECT MIN(quantity) FROM order_details;

12. SELECT AVG(quantity) AS "Average Quantity",
	MAX(quantity) AS "MAX QUANTITY",
	MIN(quantity) AS "MIN QUANTITY"
	FROM order_details
	GROUP BY orderid;

13. SELECT shipname
	FROM orders
	WHERE orderid='10290';

14. SELECT * FROM orders
	INNER JOIN customers ON orders.customerid = customers.customerid;

	SELECT * FROM orders
	LEFT JOIN customers ON orders.customerid = customers.customerid;

	SELECT * FROM orders
	RIGHT JOIN customers ON orders.customerid = customers.customerid;

15. SELECT *
	FROM employees
	WHERE reportsto IS NULL;

16. SELECT *
	FROM employees
	WHERE reportsto='2';





