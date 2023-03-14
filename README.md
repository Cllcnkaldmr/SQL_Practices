# SQL_Practices
Sql practices for the course of Patika.dev . My link is: https://app.patika.dev/cllcnkaldmr

PRACTICE 1

-- Syntax: SELECT column1 FROM table1;
-- WHERE, AND, OR, NOT, WHERE NOT;

--SELECT title, description from film;

--SELECT * FROM film
--WHERE length >60 AND length < 75;

--SELECT * FROM film
--WHERE rental_rate = 0.99 AND replacement_cost = 12.99 
--OR replacement_cost = 28.99;

--SELECT last_name from customer
--WHERE first_name = 'Mary';
--(the answer is 'Smith')


--SELECT * from film
--WHERE NOT (length > 50 AND rental_rate = 2.99 OR rental_rate = 4.99);


PRACTICE 2

--SELECT * FROM film
--WHERE replacement_cost BETWEEN 12.99 AND 16.99;

--SELECT first_name, last_name FROM actor
--WHERE first_name IN ('Penelope', 'Nick', 'Ed');

--SELECT * FROM film
--WHERE (rental_rate IN (0.99, 2.99, 4.99))
--AND (replacement_cost IN (12.99, 15.99, 28.99));


PRACTICE 3

--SELECT country FROM country
--WHERE country LIKE 'A%a';

--SELECT country FROM country
--WHERE country LIKE '_____%n';

--SELECT title FROM film
--WHERE title ILIKE '%t%t%t%t';

--SELECT * FROM film
--WHERE (title LIKE 'C%') AND length >90 AND rental_rate = 2.99;


PRACTICE 4

--SELECT DISTINCT replacement_cost FROM film;

--SELECT COUNT(DISTINCT replacement_cost) FROM film;

--SELECT COUNT(*) FROM film
--WHERE (title ~~ 'T%') AND rating = 'G';

--SELECT COUNT(*) FROM country
--WHERE country ~~ '_____';

--SELECT COUNT(*) FROM city
--WHERE city ~~* '%r';


PRACTICE 5

--SELECT title FROM film
--WHERE title LIKE '%n'
--ORDER BY length DESC
--LIMIT 5;


--SELECT title, length FROM film
--WHERE (title LIKE '%n')
--ORDER BY length
--OFFSET 5
--LIMIT 5;

--SELECT * from customer
--WHERE (store_id = 1)
--ORDER BY last_name DESC
--LIMIT 4;


PRACTICE 6

--SELECT AVG(rental_rate) FROM film;  --2.98

--SELECT COUNT(title) FROM film
--WHERE title LIKE 'C%'; --92

--SELECT * FROM film
--WHERE rental_rate = 0.99
--ORDER BY length DESC
--LIMIT 1;  --184

--SELECT COUNT(DISTINCT replacement_cost) FROM film
--WHERE length > 150;  --21 
