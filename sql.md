[mobilege /](https://github.com/mobilege/mobilege.github.io/blob/master/README.md)
[data-science /](https://github.com/mobilege/data-science/blob/master/README.md)

# SQL

#### Setup

- Book Resources: https://forta.com/books/0135182794/
- Blog: https://cierra-andaur.medium.com/sams-teach-yourself-sql-in-10-minutes-a-day-setting-up-for-success-76dd346e5dd

#### Retrieving Data
```SQL
-- Retrieving All Columns
SELECT * FROM Products;

-- Retrieving specific columns
SELECT prod_id, vend_id, prod_name FROM Products;

-- Distinct
SELECT DISTINCT vend_id FROM Products;

-- Limit
SELECT * FROM Products LIMIT 3;
```

#### Sort 
```SQL
-- Sort single column ascending

-- Sort single column descending

-- Sort two columns, first ascending, second descending
```

#### Filter (WHERE)

```SQL
-- Return records matching value

-- Return records not matching value

-- Return records matching range

-- Return records matching no value

```
