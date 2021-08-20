## データベース詳細

country_table
|属性名|型|PK|NN|FK|
|------|-------|-|-|-|
|country_id|int(3)|〇|〇||
|country_name|varchar(30)||〇||


area_table
|属性名|型|PK|NN|FK|
|------|-------|-|-|-|
|area_id|bigint(20)|〇|〇||
|area_name|varchar(50)||〇||
|country_id|int(3)||〇|〇|

pamphlet_table
|属性名|型|PK|NN|FK|
|------|-------|-|-|-|
|pamphlet_id|bigint(23)|〇|〇||
|country_id|int(3)||〇|〇|
|area_id|bigint(20)||〇|〇|
|price|int(10)||〇||
|num|int(10)||〇||
|purchas_date|date||||
|delivery_date|date||||

airplane_ticket_table
|属性名|型|PK|NN|FK|
|------|-------|-|-|-|
|ticket_id|varchar(30)|〇|〇||
|country_id|int(3)||〇|〇|
|area_id|bigint(20)||〇|〇|
|purchas_date|date||〇||
|delivery_date|date||〇||

order_table
|属性名|型|PK|NN|FK|
|------|-------|-|-|-|
|order_id|bigint(20)|〇|〇||
|customer_code|varchar(50)||〇||
|purchase_date|date||〇||

purchase
|属性名|型|PK|NN|FK|
|------|-------|-|-|-|
