1. Update the daily rate for a Mercedes car to 68.
```
update vehicle set dailyrate = 68.00 where make = 'Mercedes';
```

2. Delete a specific customer and all associated leases and payments.
```

```

3. Rename the "paymentDate" column in the Payment table to "transactionDate".
```
alter table payment rename column paymentdate to transactiondate;
```

4. Find a specific customer by email.
```
select * from customer where email = 'sarah@example.com';
```

5. Get active leases for a specific customer.
```

```

6. Find all payments made by a customer with a specific phone number.
```
select * from payment where leaseid in(select leaseid from lease where customerid in (select customerid from customer where `phoneNumber` = '555-789-1234'));
```

7. Calculate the average daily rate of all available cars.
```
select avg(dailyrate) as average_daily_rate from vehicle;
```

8. Find the car with the highest daily rate.
```
select * from vehicle where dailyrate = (select max(dailyrate) from vehicle);
```

9. Retrieve all cars leased by a specific customer.
```
select * from vehicle where `vehicleId` in (select `vehicleId` from lease where customerid = 3);
```

10. Find the details of the most recent lease.
```

```

11. List all payments made in the year 2023.
```
select * from payment where year(transactiondate) = 2023;
```

12. Retrieve customers who have not made any payments.
```

```

13. Retrieve Car Details and Their Total Payments.
```

```

14. Calculate Total Payments for Each Customer.
```

```

15. List Car Details for Each Lease.
```
select * from vehicle where `vehicleId` in (select `vehicleId` from lease group by leaseid);
```

16. Retrieve Details of Active Leases with Customer and Car Information.
```

```

17. Find the Customer Who Has Spent the Most on Leases.
```
select * from customer where customerid = (select customerid from lease where leaseid = (select leaseid from payment where amount = (select max(amount) from payment)));
```

18. List All Cars with Their Current Lease Information.
```

```
