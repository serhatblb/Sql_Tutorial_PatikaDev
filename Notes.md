# Notes

SQL = Structured Query Language
SQL declarative bildirimsel bir programlama dilidir.
> **Kullanım şekli:**
`SELECT title FROM book WHERE page_number > 200; `

#### PostgreSQL
-   Açık kaynak kodlu
-   Çeşitli veri tipi desteği
-   Güçlü dökümantasyon ve topluluk desteği
-   Tüm işletim sistemlerine uygunluk
-   ACID uyumluluk
-   Güvenlidir
-   Büyük verilerle kolay çalışma
#

#### SELECT
Sorgu (Query)
SQL komutlarını içeren sorgu cümleleridir.
> **Kullanım şekli:**
> `SELECT <sütun_adı>, <sütun_adı>, ... FROM <tablo_adı>;`

> **Ornek:**
> `SELECT first_name, last_name FROM actor;`
#

####  WHERE
SELECT komutu ile yaptığımız çalışmalarda bizler tüm sütunların veya ilgili sütunlarda bulunan verilerin tamamını çekmek isteriz. Çoğu durumda ise verilerin tamamını değil belirli koşulları sağlayan verileri görmek isteriz. Bunun için **WHERE** anahtar kelimesini kullanırız.
> **Kullanım şekli:**
> `SELECT <sütun_adı>, <sütun_adı>, ... FROM <tablo_adı> WHERE <koşul>;`

> **Ornek:**
> `SELECT title, replacement_cost FROM film WHERE replacement_cost = 14.99;`
#
####  AAA
Acıklama
> **Kullanım şekli:**
> `SELECT <sütun_adı>, <sütun_adı>, ... FROM <tablo_adı> WHERE <koşul>;`

> **Ornek:**
> `SELECT title, replacement_cost FROM film WHERE replacement_cost = 14.99;`
#
####  AAA
Acıklama
> **Kullanım şekli:**
> `SELECT <sütun_adı>, <sütun_adı>, ... FROM <tablo_adı> WHERE <koşul>;`

> **Ornek:**
> `SELECT title, replacement_cost FROM film WHERE replacement_cost = 14.99;`
#