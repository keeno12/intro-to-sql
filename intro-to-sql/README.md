# intro to SQL  

## short URL to this repo https://github.com/keeno12/into-to-sql

## Setting up your computer:

- Open your web browser. I'll be using [chrome](https://www.google.com/chrome/), but  you can use [Safari](https://www.apple.com/safari/) or [Opera](https://www.opera.com/)(browsers that support [Web SQL](https://en.wikipedia.org/wiki/Web_SQL_Database)).
- to speed up learning we're going to use an [online editor and database](https://www.w3schools.com/sql/trysql.asp?filename=trysql_select_all) for SQL from [W3Schools](https://www.w3schools.com/).

That was easy!


## Galvanize

### Welcome to Galvanize!

We create a technology ecosystem for learners, entrepreneurs, startups, and established companies to meet the needs of the rapidly changing digital world.

We're an awesome community!!!


If you have any questions about Galvanize immersive offerings in Data Science or Web Engineering, you can also email us at [learn@galvanize.com](mailto:learn@galvanize.com)


## About me:
Hello I'm [Keenan Olsen](https://linkedin.com/in/keenanolsen). I'm a Developer Evangelist at Galvanize San Francisco. Previously I've worked as a software developer with Startups and Agencies in Boulder, CO and here in San Francisco.

*caveat* I'm not an Galvanize instructor, they're much better at teaching than I am!

If you have an event you would like to see or put on let me know! I'm always looking for ideas. Talk to me after the workshop or find me online at one of these:

- Website: [keenanolsen.me](https://keenanolsen.me)
- Twitter: [@KeenanOlsen](https://twitter.com/@keenanolsen)
- LinkedIn: [Keenan Olsen](https://www.linkedin.com/in/keenanolsen/)
- Email: [keenan.olsen@galvanize.com](mailto:keenan.olsen@galvanize.com)


## About you!

Give a quick Intro!

- Whats your name?
- Whats your background?
- Why are you interested in SQL and data?

One of the best things about these in person workshops is being able to meet new people! Talk to each other!


## What this workshop is

A super friendly introduction to SQL No previous experience expected!

You can't learn EVERYTHING in ~2 hours. But you can learn enough to get excited and comfortable to keep working and learning on your own! Come to our almost weekly code hours [meetups](https://www.meetup.com/SF-Data-Science/) to ask questions if you get stuck and show off what you've been working on!

- This course is for absolute beginners
- Ask Questions!
- Answer Questions!
- Help others when you can
- Its ok to get stuck, just ask for help!
- Feel free to move ahead
- Be patient and nice


## Why is data important

### What is Data?
Data is information. Imagine a phonebook with hundreds of people and businesses.

### What is a Databases?

A database is computerized storage of data. Imagine an organized digital collections of the same people and businesses from the above phone book.

###### Examples

Examples of products using databases.

- Dynamic sites
	- Facebook
	- Gmail  
- Mobile apps
	- Uber
	- Snapchat
- Data for recommendations
	- Netflix
	- Amazon products
- Item Tracking
	- Library
	- UPS

Some Professional Roles that work with databases:

- Web Developer
- Data Analysts
- Data scientist
- Database Admin


## What is SQL?

Pronounced `S` `Q` `L` or `Sequel`. Either way is fine!

SQL stands for Structured Query Language. This is the language and syntax we will use to interact with SQL databases.

When we return and search data from a database we call it Querying.

Common SQL Databases:

Each of these databases can be Queried using the SQL programming Language.

- MySQL
- PostgreSQL
- Microsoft SQL
- SQLite
- Oracle

*Note:* There are some slight differences to each database, but most of the SQL commands we're going to cover will be the same or very similar.
 you can read more about the difference on common SQL databases [here](https://www.w3schools.com/sql/sql_ref_mysql.asp).

Some other popular databases to keep an eye out for as you continue to learn:

- MongoDB
- Couchbase
- Redis

These are often referred to noSQL databased. Read more about noSQL [here](https://www.mongodb.com/nosql-explained)


<!--#### Where SQL used?

#### What is an ORM?

ORM stands for Object relation model
-->


## What is a relational database?

There are two major components in a database:

- Data(Information Stored) and Schema(How the data is organized)
- Sections. Also called tables. This how the data get structured.


##### Tables
You can think of tables as spreadsheets:


| Column ↓  | Column ↓   |  Column ↓  |
|---|---|---|
| Row →   |   |   |
| Row →   |   |   |
| Row →   |   |   |

##### Table Organization

Usually separate tables contain data for a specific type of thing:

If we look at [w3schools](https://www.w3schools.com/sql/trysql.asp?filename=trysql_select_all) again you can see all the different tables in the database

![alt text](img/tables.png "Tables")


Orders table:

| OrderID  |  	CustomerID | 	EmployeeID  | OrderDate  |  ShipperID |
|---|---|---|---|---|
| 10248  | 90  |  5 | 1996-07-04  | 	3  |
| 10249  |  81 |  6 |  1996-07-05 |  1 |
|  10250 | 34  | 4  |  1996-07-08 |  2 |


Products Tables:

| ProductID  | ProductName  | SupplierID  | CategoryID  |  Unit | Price|
|---|---|---|---|---|---|
| 1  |  Chais |  1 |  1 |  10 boxes x 20 bags | 18  |
|  2 |  Chang |  1 |  1 | 24 - 12 oz bottles  | 19 |
|  3 | Aniseed Syrup  | 1  | 2  |  12 - 550 ml bottles | 10  |


<!--Filter data table example:

Rearrange table example:-->

Having multiple tables storing data can seem complicated at first, why not have everything in one giant table?

Each table can have relationships with each other, instead of repeating the same product how ever many times someone buys it, we can instead reference back to that product in a separate table.

Again, don't worry if this is a bit confusing! It will make more sense as we go!


The same database can be used in different ways across applications at the same time.

- Website could be pulling data to show your purchase history
- An analyst could be pulling the data to learn what the most popular item is




### Data types

data types for table columns are defined in the schema

The most common data types are:

- Text (Names, Descriptions)
- Numeric (cost, age, weight, quantity)
- Dates (Dates and time)

Its important to have the correct data type for your data. This ensures that sorting and calculations work properly. We won't be setting up a database in this workshop, but it something to keep in mind when you do!

*Note:* Data types may change depending on which database you're using.


We could spend a whole workshop discussing databases, but we're going to focus on querying language SQL for the remainder of this workshop.

Learn more about databases on your own [here](https://www.w3schools.com/sql/sql_create_db.asp)!

If you would like to see a workshop more focused on Databases and how create them let me know!



## lets do some SQL!

Visit [w3schools](https://www.w3schools.com/sql/trysql.asp?filename=trysql_select_all) and navigate to the SQL section.


### Querying

Important first step is to understand your data.

- How is it structured?
- What does it represent?


Lets do some different types querying to figure this out!

Lets take a look at all the categories of products we have

`SELECT * FROM Categories;`

Lets see how many customers we have?

`SELECT COUNT(*) FROM Customers;`

Lets take a look at our orders

`SELECT * FROM Orders;`

Lets rearrange the orders by date

*Note:* When we query this isn't actually changing the database. You're just choosing what and how to look at the data.

```
SELECT * FROM Orders
ORDER BY OrderDate DESC;
```
ASC = Ascending
DESC = Descending

Neat! Lets see which customer made that top order (most recent)! We will take the value from the CustomerID column.

```
SELECT * FROM customers
WHERE CustomerID = 66;
```

Cool! We can also query for matches in multiple columns

```
SELECT * FROM OrderDetails
WHERE ProductID = 14 AND Quantity < 10;
```

We can also filter columns by more than one value.

```
SELECT * FROM OrderDetails
WHERE ProductID = 14 OR ProductID = 42;
```


So far we have been returning all the columns of a record that match our query. What if we want to only look at a few of them?

Instead of using `*` to select all we can put in the specific columns we want returned. We can also put them in different order!

```
SELECT Country, city, CustomerName FROM Customers;
```
Lets order by Ascending order (A-Z) of Country Name

```
SELECT Country, city, CustomerName FROM Customers
ORDER BY Country ASC;
```

Lets See just a list of countries
Using `DISTINCT`. Which will just return one instance.

Run the query below with and without `DISTINCT` to see the difference.

```
SELECT DISTINCT Country FROM Customers
ORDER BY Country ASC;

```


Sometimes we want to filter by records that contain values or characters that are not an exact match.

What customers have a name starting with `A`?

```
SELECT * FROM Customers
WHERE CustomerName LIKE 'A%';
```

- 'A%' Starts with an A
- '%A' Ends with an A
- '%A%' Contains an A

Read more types of way to filter [here](https://www.w3schools.com/sql/sql_like.asp).


## Functions

If you've used excel you'll probably be familiar with some of these functions.


- SUM() `SELECT SUM(Quantity) FROM OrderDetails;`
- MAX() `SELECT ProductID, ProductName, MAX(Price) FROM Products;`
- MIN() `SELECT ProductID, ProductName, MIN(Price) FROM Products;`
- AVG() `SELECT AVG(Price) FROM Products;`
- COUNT() `SELECT COUNT(*) FROM Customers;`


### Changing Data to the database

So far we've only been looking at our data in different ways, which is super useful for answering questions, but lets actually make some changes to the database!


#### Insert into

```
SELECT * FROM Customers;
```

```
INSERT INTO Customers (CustomerName, City, Country)
VALUES ('Keenan', 'San Francisco', 'USA');
```

```
SELECT * FROM Customers;
```

##### What's Null?
You should notice that some of the sections on our new row contain the word `null`.
In SQL you can think of `null` means that the cell contains no value.


#### Update

```
SELECT * FROM Customers;
```

```
UPDATE Customers
SET ContactName='Keenan', City='San Francisco'
WHERE CustomerID=1;
```

```
SELECT * FROM Customers;
```

Its common to select and update more than one single row by ID.

```
SELECT * FROM Customers
WHERE CustomerName LIKE 'A%'
```

```
UPDATE Customers
SET ContactName='I started with an A', City='A town'
WHERE CustomerName LIKE 'A%'
```

```
SELECT * FROM Customers
WHERE CustomerName LIKE 'A%'
```

#### Delete

```
SELECT * FROM Customers;
```

```
DELETE FROM Customers
WHERE CustomerName='Keenan';
```

```
SELECT * FROM Customers;
```


### Joins

We're not going to go super deep into joins in this workshop and they can be a bit tricky to understand, so don't worry if you don't quite get it yet! Read about and practice them further [here](https://www.w3schools.com/sql/sql_join.asp).

This of it as essentially joining tables together. We're then returning combined table for use to use.

```
SELECT Orders.OrderID, Customers.CustomerName, Orders.OrderDate
FROM Orders
INNER JOIN Customers ON Orders.CustomerID=Customers.CustomerID;
```


By default when you just use 'join' we are creating a inner join. Read more about different joins [here](https://www.w3schools.com/sql/sql_join.asp)
.

Find a helpful graph on joins [here](https://stackoverflow.com/questions/565620/difference-between-join-and-inner-join).


#### Group by

Instead of getting each row, sometimes we want to group them by

```
SELECT COUNT(ShipperID), ShipperID FROM [Orders]
GROUP by ShipperID;
```


Lets do something useful with grouping. Lets find out which shipper has been used the most.

```
SELECT COUNT(Orders.ShipperID), Orders.ShipperID, Shippers.ShipperName
FROM [Orders]
JOIN Shippers ON Orders.ShipperID=Shippers.ShipperID
GROUP by Orders.ShipperID
ORDER BY COUNT(Orders.ShipperID) DESC;
```

### Comments

Comments are awesome. When you're writing more complex code / queries use comments to help you remember what that piece of code is doing!


```
-- SQL Comment
SELECT * FROM Customers;
```


### Recap!





## Questions
Knowing what we just learned lets try to answer some questions about our data!

- How many items have we shipped?
- What is the most expensive item?
- What is the most popular item?
<!--- Which customer has spent the most money?-->
- Which customer has returned the most?
- Whats the most popular category?

You can find some of the answers at the bottom of this repo to help get you going!


## Keep Learning!!!

Resources:
- [w3schools](https://www.w3schools.com/sql/)
- [sqlzoo](https://sqlzoo.net/)
- [Datacamp](https://www.datacamp.com/courses/intro-to-sql-for-data-science)
- [Read about what an ORM (Object-relational mapping) is](https://stackoverflow.com/questions/1279613/what-is-an-orm-and-where-can-i-learn-more-about-it)
-[pgexercises](https://pgexercises.com/questions/basic/)

Setup an actual database on your computer!


## Upcoming Events!
We host so many events! check out our [calendar](https://www.galvanize.com/san-francisco/events)

[Learn code](https://www.meetup.com/learn-to-code-san-francisco/). Thats this meetup! We do workshops and community programming nights! Keep an eye out for more events coming to San Francisco soon!

Upcoming Learn to code [events](https://www.meetup.com/SF-Data-Science/):


## What is Galvanize?

#### Immersive Bootcamp
- [Data Science](https://www.galvanize.com/san-francisco/data-science) - 1/22/2019
- [Software Engineer](https://www.galvanize.com/san-francisco/web-development) - 10/5/2018

#### Part-Time Courses

- [Python Accelerated Evening Course](https://www.galvanize.com/seattle/web-development-foundations) - 10/29/2018
- [2 Day Statistics Short-Course](https://www.galvanize.com/seattle/data-analytics) - 12/04/2018


#### Co-working Space
[work in our building!](https://www.galvanize.com/entrepreneur)


#### We are a community!

## Questions:
Please feel free to reach out to me with any questions!

This was only my 2nd time running this workshop, help improve it by giving me feedback :)

- Website: [keenanolsen.me](https://keenanolsen.me)
- Twitter: [@KeenanOlsen](https://twitter.com/@keenanolsen)
- LinkedIn: [Keenan Olsen](https://www.linkedin.com/in/keenanolsen/)
- Email: [keenan.olsen@galvanize.com](mailto:keenan.olsen@galvanize.com)

THANK YOU FOR HAVING ME SAN FRANCISCO!

Questions about education at Galvanize SF email [learn@galvanize.com](mailto:learn@galvanize.com)

---------
## Query Answers
Answers to the Questions Section:

- Q: How many items have we shipped?
	- A: 12,743
	- `SELECT SUM(Quantity) FROM OrderDetails;`


- Q: What is the most expensive item?
	- A: Côte de Blaye
	- `SELECT ProductID, ProductName, MAX(Price) FROM Products;`

- Q: What is the most popular item?
	- A: Gorgonzola Telino

```
SELECT SUM(OrderDetails.Quantity), Products.ProductName, OrderDetails.ProductID
FROM OrderDetails
JOIN Products ON OrderDetails.productID=Products.ProductID
GROUP BY ProductName
ORDER BY SUM(OrderDetails.Quantity) DESC;
```


- Which customer has returned the most?
	- A: Ernst Handel

```
SELECT Customers.CustomerName, COUNT(Customers.CustomerID)
FROM Orders
JOIN Customers ON Orders.CustomerID=Customers.CustomerID
JOIN OrderDetails ON Orders.OrderID=OrderDetails.OrderID
GROUP BY Customers.CustomerID
ORDER BY COUNT(Customers.CustomerID) DESC;
```
