## データベース詳細

d_purchase
|属性名|型|PK|NN|FK|
|------|-------|-|-|-|
|order_id|bigint(20)|〇|〇||
|customer_code|varchar(50)||〇||
|purchase_date|date||〇||
|total_price|int(11)||〇||

d_purchase_detail
|属性名|型|PK|NN|FK|
|------|-------|-|-|-|
|detail_id|bigint(20)|〇|〇||
|order_id|bigint(20)|〇|〇|〇|
|item_code|int(11)||〇||
|price|int(11)||〇||
|num|int(11)||〇||

m_customers
|属性名|型|PK|NN|FK|
|------|-------|-|-|-|
|customer_code|varchar(50)|〇|〇||
|pass|varchar(50)|〇|〇|〇|
|name|varchar(20)||〇||
|address|varchar(100)||〇||
|tel|varchar(20)||〇||
|mail|varchar(100)||〇||
|del_flag|int(11)||||
|reg_date|date||〇||
