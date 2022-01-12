# List Customer And Product Without Sale

Need to show the following columns (3) using UNION to return:

- All customers who do not have an invoice
- All products that were not sold

1. Category: Is this related to "customer" or "product"? Print "customer or "product"
2. ID: Customer.id (category="customer") or product.id (category="product")
3. Name: customer.customer_name (category="customer") or product.product_name (category="product")

Tables:

- Customer

id
customer_name
city_id
customer_address
contact_person
email
phone

- Product

id
sku
product_name
product_description
current_price
quantity_in_stock

- Invoice

id
invoice_number
customer_id
user_account_id
total_price
time_issued
time_due
time_paid
time_canceled
time_refunded

- Invoice_Item

id
invoice_id
product_id
quantity
price
line_total_price