[mobilege /](https://github.com/mobilege/mobilege.github.io/blob/master/README.md)
[data-science /](https://github.com/mobilege/data-science/blob/master/README.md)

# SQL

- Book Resources: https://forta.com/books/0135182794/
- Blog: https://cierra-andaur.medium.com/sams-teach-yourself-sql-in-10-minutes-a-day-setting-up-for-success-76dd346e5dd

#### 1. Retrieving Data (SELECT)
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

#### 2. Sorting Data (SORT) 
```SQL
-- Sort single column ascending

-- Sort single column descending

-- Sort two columns, first ascending, second descending
```

#### 3. Filtering Data (WHERE)
```SQL
-- Return records matching value

-- Return records not matching value

-- Return records matching no value

-- Return records BETWEEN range

-- Return records IN range
```

#### 4. Advanced Filtering with wildcards (LIKE)
```
-- Return Records that begins with, ends with and contains a specific string.

-- Return Records that begins with, or ends with any (single) character where the rest of the string is given.

-- Return Records that begins with, or ends with one of two given special characters, where the rest of the string is also given.
```

#### 5. Using Data Manipulation Functions

#### 6. Summarizing Data (Aggregate Functions)

#### 7. Grouping Data

#### 8. Joining Tables

#### 9. Inserting, Updating & Deleting Records

#### 10. Creating, Updating and Deleting Tables
