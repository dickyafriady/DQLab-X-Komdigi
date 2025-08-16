# Project Data Analysis for Retail: Sales Performance Report
## Dataset Brief
ataset yang digunakan berisi transaksi dari tahun 2009 sampai dengan tahun 2012 dengan jumlah raw data sebanyak 5500, termasuk di dalamnya order status yang terbagi menjadi order finished, order returned dan order cancelled.
Adapun dataset yang sudah diberikan dan akan digunakan pada project ini berisi data sebagai berikut.

1. OrderID
2. Order Status
3. Customer
4. Order Date
5. Order Quantity
6. Sales
7. Discount %
8. Discount
9. Product Category1
10. Product Sub-Category

Nama tabel yang akan digunakan pada project ini adalah dqlab_sales_store.

## Petunjuk Penyelesaian Project
Untuk menyelesaikan project, maka kita akan mengetikkan code yang perlu disubmit untuk dicek jawabannya benar atau salah.
Dari data yang sudah diberikan, dari pihak manajemen DQLab store ingin mengetahui:

1A. Overall perofrmance DQLab Store dari tahun 2009 - 2012 untuk jumlah order dan total sales order finished.
1B. Overall performance DQLab by subcategory product yang akan dibandingkan antara tahun 2011 dan tahun 2012.

2A. Efektifitas dan efisiensi promosi yang dilakukan selama ini, dengan menghitung burn rate dari promosi yang dilakukan overall berdasarkan tahun.
2B. Efektifitas dan efisiensi promosi yang dilakukan selama ini, dengan menghitung burn rate dari promosi yang dilakukan overall berdasarkan sub-category.

 Setelah melihat hasil analisa di Sub Bab 1 dan 2, selanjutnya dilakukan analisa terhadap customer DQLab. Analisa dari sisi customer dengan menggunakan metrics:
3A. Analisa terhadap customer setiap tahunnya.
3B. Analisa terhadap jumlah customer baru setiap tahunnya.
3C. Cohort untuk mengetahui angka retention customer tahun 2009


## _Overall Performance by Year_
Buatlah Query dengan menggunakan SQL untuk mendapatkan total penjualan (sales) dan jumlah order (number_of_order) dari tahun 2009 sampai 2012 (years). 
```sh
SELECT 
    YEAR(order_date) AS years,
    SUM(sales) AS sales,
    COUNT(order_quantity) AS number_of_order
FROM 
    dqlab_sales_store
WHERE 
    order_status = 'Order Finished' AND
    YEAR(order_date) BETWEEN 2009 AND 2012
GROUP BY 
    YEAR(order_date)
ORDER BY 
    years;
```

## _Overall Performance by Product Sub Category_
Buatlah Query dengan menggunakan SQL untuk mendapatkan total penjualan (sales) berdasarkan sub category dari produk (product_sub_category) pada tahun 2011 dan 2012 saja (years) 

```sh
SELECT 
    YEAR(order_date) AS years,
    product_sub_category,
    SUM(sales) AS sales
FROM 
    dqlab_sales_store
WHERE 
    order_status = 'Order Finished' AND
    YEAR(order_date) IN (2011, 2012)
GROUP BY 
    YEAR(order_date), product_sub_category
ORDER BY 
    years, sales DESC;
```

## _Promotion Effectiveness and Efficiency by Years_
Pada bagian ini kita akan melakukan analisa terhadap efektifitas dan efisiensi dari promosi yang sudah dilakukan selama ini. Efektifitas dan efisiensi dari promosi yang dilakukan akan dianalisa berdasarkan Burn Rate yaitu dengan membandigkan total value promosi yang dikeluarkan terhadap total sales yang diperoleh. DQLab berharap bahwa burn rate tetap berada diangka maskimum 4.5%.

_Formula untuk burn rate : (total discount / total sales) * 100_

Buatkan Derived Tables untuk menghitung total sales (sales) dan total discount (promotion_value) berdasarkan tahun(years) dan formulasikan persentase burn rate nya (burn_rate_percentage).
```sh
SELECT YEAR(order_date) as years, 
    SUM(sales) as sales,
    SUM(discount_value) as promotion_value,
    ROUND(SUM(discount_value) / SUM(sales) * 100, 2) as burn_rate_percentage
FROM dqlab_sales_store
WHERE
	order_status LIKE 'Order Finished'
GROUP BY
    years
ORDER BY
    years;
```
## _Promotion Effectiveness and Efficiency by Product Sub Category_
Pada bagian ini kita akan melakukan analisa terhadap efektifitas dan efisiensi dari promosi yang sudah dilakukan selama ini seperti pada bagian sebelumnya. 

Akan tetapi, ada kolom yang harus ditambahkan, yaitu : product_sub_category dan product_category.
Notes :
1. Data yang ditampilkan hanya untuk tahun 2012
2. Contoh output di atas hanya 5 baris pertama dari output yang diharapkan
```sh
SELECT YEAR(order_date) as years, 
    product_sub_category,
    product_category,
    SUM(sales) as sales,
    SUM(discount_value) as promotion_value,
    ROUND(SUM(discount_value) / SUM(sales) * 100, 2) as burn_rate_percentage
FROM dqlab_sales_store
WHERE
	order_status LIKE 'Order Finished' 
    AND YEAR(order_date) = '2012'
GROUP BY
    years,
    product_sub_category,
    product_category
ORDER BY
    sales DESC;
```

## _Customers Transactions per Year_
DQLab Store ingin mengetahui jumlah customer (number_of_customer) yang bertransaksi setiap tahun dari 2009 sampai 2012 (years).
```sh
SELECT YEAR(order_date) as years,
	COUNT(DISTINCT(customer)) as number_of_customer
FROM dqlab_sales_store
WHERE YEAR(order_date) BETWEEN '2009' AND '2012'
	AND order_status LIKE 'Order Finished'
GROUP BY years	
ORDER BY years;
```
