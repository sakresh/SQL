# This file contains the queries that were used to create the tables

## Creation of the Customers Table
``` create table customers(customer_id int primary key, name varchar(255), email varchar(255), password varchar(255)); ```

## Creation of the Products Table
``` create table products(product_id int primary key, name varchar(255), price int, description varchar(255), stockQuantity int); ```

## Creation of the Cart Table
``` create table cart(cart_id int primary key, customer_id int, foreign key(customer_id) references customers(customer_id), product_id int, foreign key(product_id) references products(product_id), quantity int); ```

## Creation of the Orders Table
``` create table orders(order_id int primary key, customer_id int, foreign key(customer_id) references customers(customer_id), order_date date, total_price int, shipping_address varchar(255)); ```

## Creation of the Order Items Table
``` create table order_items(order_item_id int primary key, order_id int, foreign key(order_id) references orders(order_id), product_id int, foreign key(product_id) references products(product_id), quantity int); ```
