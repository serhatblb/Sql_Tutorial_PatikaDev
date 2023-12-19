# Genel Tekrar

1. film tablosundan 'K' karakteri ile başlayan en uzun ve replacenet_cost u en düşük 4 filmi sıralayınız.
```
SELECT title,length, replacement_cost FROM film 
WHERE title LIKE 'K%' 
ORDER BY length DESC, replacement_cost LIMIT 4;
```

2. film tablosunda içerisinden en fazla sayıda film bulunduran rating kategorisi hangisidir?
```
SELECT rating, COUNT(*) AS film_sayisi FROM film
GROUP BY rating
ORDER BY film_sayisi DESC
LIMIT 1;
```

3. customer tablosunda en çok alışveriş yapan müşterinin adı nedir?
```
SELECT customer.first_name, customer.last_name, count(*) FROM customer
INNER JOIN payment on customer.customer_id = payment.customer_id
GROUP BY customer.first_name, customer.last_name 
ORDER BY COUNT(*) DESC LIMIT 1;
```

4. category tablosundan kategori isimlerini ve kategori başına düşen film sayılarını sıralayınız.
```
SELECT category.name,COUNT(*) AS kategori_basina_dusen_film_sayisi FROM category JOIN film_category 
ON film_category.category_id = category.category_id
JOIN film ON film.film_id = film_category.film_id
GROUP BY category.name ORDER BY kategori_basina_dusen_film_sayisi,
```

5. film tablosunda isminde en az 4 adet 'e' veya 'E' karakteri bulunan kaç tane film vardır?
```
SELECT COUNT(*) FROM film WHERE title ILIKE '%e%e%e%e%'; 
```