```SQL
SELECT 
ood.order_id, order_purchase_timestamp, order_delivered_customer_date, price, freight_value, payment_sequential, payment_type, payment_installments, payment_value, product_category_name, customer_city, customer_state,
    pcnt.column1 AS product_category_name_portuguese,
    COALESCE(pcnt.column2, 'Unknown') AS product_category_name_english
FROM 
    olist_orders_dataset AS ood
LEFT JOIN 
    olist_order_items_dataset AS ooid
ON 
    ood.order_id = ooid.order_id
LEFT JOIN 
    olist_sellers_dataset AS osd
ON 
    ooid.seller_id = osd.seller_id
LEFT JOIN 
    olist_order_payments_dataset AS oopd
ON 
    ood.order_id = oopd.order_id
LEFT JOIN 
    olist_products_dataset AS opd
ON 
    ooid.product_id = opd.product_id 
LEFT JOIN 
    olist_customers_dataset AS ocd
ON 
    ood.customer_id = ocd.customer_id
LEFT JOIN 
    olist_geolocation_dataset AS ogd
ON 
    osd.seller_zip_code_prefix = ogd.geolocation_zip_code_prefix
LEFT JOIN 
    olist_order_reviews_dataset AS oord
ON 
    oord.order_id = ood.order_id
LEFT JOIN 
    product_category_name_translation AS pcnt 
ON 
    opd.product_category_name = pcnt.column1;
```
