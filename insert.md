# This file contains the queries that were used to insert elements into the tables created

## Inserting items to the Products Table
```
insert into products values(1, 'Laptop', 800, 'Higt-performance laptop', 10), (2, 'Smartphone', 600, 'Latest smartphone', 15), (3, 'Tablet', 300, 'Portable Tablet', 20), (4, 'Headphones', 150, 'Noise-canceling', 30),(5, 'TV', 900, '4K Smart TV', 5), (6,'Coffee Maker', 50, 'Automatic coffee maker', 25), (7, 'Refrigerator', 700, 'Energy-efficient', 10), (8, 'Microwav Oven', 80, 'Countertop microwave', 15), (9, 'Blender', 70, 'High-speed blender', 20), (10, 'Vacuum Cleaner', 120, 'Bagless vacuum cleaner', 10);
```

## Inserting items to the Customers Table
```
insert into customers values(1, 'JohnDoe', 'johndoe@example.com', '123'), (2, 'JaneSmith', 'janesmith@example.com', '456'), (3, 'RobertJohnson', 'robert@example.com', '789'), (4, 'SarahBrown', 'sarah@example.com', '012'), (5, 'DavidLee', 'david@example.com', '345'), (6, 'LauraHall', 'laura@example.com', '678'), (7, 'MichaelDavis', 'michael@example.com', '901'), (8, 'EmmaWilson', 'emma@example.com', '234'), (9, 'WilliamTaylor', 'william@example.com', '567'), (10,'OliviaAdams', 'olivia@example.com','890');
```

## Inserting items to the Cart Table
```
insert into cart values(1, 1, 1, 2), (2, 1, 3, 1), (3, 2, 2, 3), (4, 3, 4, 4), (5, 3, 5, 2), (6, 4, 6, 1), (7, 5, 1, 1), (8, 6, 10, 2), (9, 6, 9, 3), (10, 7, 7, 2);
```

## Inserting items to the Orders Table
```
insert into orders values (1, 1, '2023-01-05', 1200, '123 Main St, City'), (2, 2, '2023-02-10', 900, '456 Elm St, Town'), (3, 3, '2023-03-15', 300, '789 Oak St, Village'), (4, 4, '2023-04-20', 150, '101 Pine St, Suburb'), (5, 5, '2023-05-25', 1800, '234 Cedar St, District'), (6, 6, '2023-06-30', 400, '567 Birch St, County'), (7, 7, '2023-07-05', 700, '890 Maple St, State'), (8, 8, '2023-08-10', 160, '321 Redwood St, Country'), (9, 9, '2023-09-15', 140, '432 Spruce St, Province'), (10, 10, '2023-10-20', 1400, '765 Fir St, Territory');
```

## Inserting items to the Order_items Table
```
insert into order_items values(1, 1, 1, 2), (2, 1, 3, 1), (3, 2, 2, 3), (4, 3, 5, 2), (5, 4, 4, 4), (6, 4, 6, 1), (7, 5, 1, 1), (8, 5, 2, 2), (9, 6, 10, 2), (10, 6, 9, 3);
```
