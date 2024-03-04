## 1. Update refrigerator product price to 800.
```
update products set price = 800 where name = 'Refrigerator';
```

## 2. Remove all cart items for a specific customer.
```

```

## 3. Retrieve Products Priced Below $100.
```
select * from products where price < 100;
```

## 4. Find Products with Stock Quantity Greater Than 5.
```
select * from products where stockQuantity > 5;
```

## 5. Retrieve Orders with Total Amount Between $500 and $1000.
```
select * from orders where total_price between 500 and 1000;
```

## 6. Find Products which name end with letter ‘r’.
```
select * from products where name like '%r';
```

## 7. Retrieve Cart Items for Customer 5.
```
select * from cart where customer_id = 5;
```

## 8. Find Customers Who Placed Orders in 2023.
```

```

## 9. Determine the Minimum Stock Quantity for Each Product Category.
```

```

## 10. Calculate the Total Amount Spent by Each Customer.
```
select sum(total_price) as total_price from orders group by customer_id;
```

## 11. Find the Average Order Amount for Each Customer.
```
select avg(total_price) as average_amount from orders group by customer_id;
```

## 12. Count the Number of Orders Placed by Each Customer.
```
select customer_id, count(cart_id) as NumberOfOrdersPlacedByEachCustomers from cart group by customer_id;

```

## 13. Find the Maximum Order Amount for Each Customer.
```

```

## 14. Get Customers Who Placed Orders Totaling Over $1000.
```
select * from orders where total_price >= 1000;

```

## 15. Subquery to Find Products Not in the Cart.
```
select * from products where product_id not in (select product_id from cart);
```

## 16. Subquery to Find Customers Who Haven't Placed Orders.
```
select * from customers where customer_id not in (select customer_id from cart);
```

## 17. Subquery to Calculate the Percentage of Total Revenue for a Product.
```

```

## 18. Subquery to Find Products with Low Stock.
```
select * from products where stockQuantity < 10; [Assume that the products having stock less than 10 are considered to have low stock quantity]
```

## 19. Subquery to Find Customers Who Placed High-Value Orders
```
select * from customers where customer_id in (select customer_id from orders where total_price > 1000); [Assume that the customers who placed orders more than $1000 are considered to have purchased high valued products]
```
