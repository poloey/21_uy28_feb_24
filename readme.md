##  fetching data from table using pivot table

~~~sql
select products.title, categories.name from product_category
join products on products.id = product_category.product_id
join categories on categories.id = product_category.category_id
~~~

## wild card (%) for searching data from database

~~~php
select * from products where title='core i5'
# wild card
select * from products where title like 'core%'
select * from products where title like '%ore%'
select * from products where title like '_ore%'
~~~

## limit and offset  (for adding pagination in webpage)

~~~php
select * from products limit 5;
select * from products limit 5 offset 10;
# or
select * from products limit 10, 5;
~~~



