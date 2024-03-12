## Creating the Vehicle table
```
create table vehicle(vehicleId int primary key, make varchar(255), model varchar(255), year year, dailyrate int, stat int, passengerCapacity int, enginecapacity int);
```

## Creating the Customer table
```
create table customer(customerid int primary key, firstName varchar(255), lastName varchar(255), email varchar(255), phoneNumber varchar(255));
```

## Creating the Lease table
```
create table lease(leaseid int primary key, vehicleId int, foreign key(vehicleId) references vehicle(vehicleId), customerid int, foreign key(customerid) references customer(customerid), startDate date, endDate date, type varchar(255));
```

## Creating the Payment table
```
create table payment(paymentid int primary key, leaseid int, foreign key(leaseid) references lease(leaseid),paymentdate date, amount decimal(10, 3));
```

