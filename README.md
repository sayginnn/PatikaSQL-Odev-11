# PatikaSQL-Odev-11

-- 1. Tüm verileri sıralama

SELECT first_name FROM actor
UNION ALL
SELECT first_name FROM customer;

-- 2. Kesişen verileri sıralama

SELECT first_name FROM actor
INTERSECT ALL
SELECT first_name FROM customer;

-- 3. İlk tabloda bulunan ancak ikinci tabloda bulunmayan verileri sıralama

SELECT first_name FROM actor
EXCEPT ALL
SELECT first_name FROM customer;
