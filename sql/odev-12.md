Aşağıdaki sorgu senaryolarını dvdrental örnek veri tabanı üzerinden gerçekleştiriniz.



1. film tablosunda film uzunluğu length sütununda gösterilmektedir. Uzunluğu ortalama film uzunluğundan fazla kaç tane film vardır?
```sql
SELECT COUNT(length) from film 
WHERE length> (
	SELECT AVG(length) from film
);
```
2. film tablosunda en yüksek rental_rate değerine sahip kaç tane film vardır?
```sql
SELECT COUNT(rental_rate) FROM film
WHERE rental_rate= (
SELECT MAX(rental_rate) FROM film
);

```
3. film tablosunda en düşük rental_rate ve en düşün replacement_cost değerlerine sahip filmleri sıralayınız.
```sql
SELECT title,rental_rate, replacement_cost FROM film
WHERE rental_rate=
 (SELECT MIN(rental_rate) FROM film)
 OR 
 replacement_cost=
(SELECT MIN(replacement_cost) FROM film)
ORDER BY rental_rate,replacement_cost;
```
4. payment tablosunda en fazla sayıda alışveriş yapan müşterileri(customer) sıralayınız.
```sql
SELECT first_name, last_name, amount FROM payment
INNER JOIN customer 
ON payment.customer_id=customer.customer_id
WHERE payment.amount=
(
SELECT MAX(amount) FROM payment
);
```
