```
select 'customer' as category, c.id as id, customer_name as name
     from customer c
     left join invoice i on c.id = i.customer_id
     where i.id is null 

union

select 'product' as category, p.id as id, product_name as name
        from product p
        left join invoice_item ii on p.id = ii.product_id
        where ii.id is null;
```