# SQL-Data-Extraction-From-DB

## Overview

This project demonstrates basic data extraction and handling using SQL queries. The focus is on retrieving and analyzing data from a relational database with straightforward SQL operations.

## Features

- **Data Extraction**:
  - Simple `SELECT` queries to retrieve specific columns.
  - Use of `SUM` and `GROUP BY` for basic data aggregation.

- **Basic Data Handling**:
  - Filtering data using `WHERE`.
  - Aggregating results with `GROUP BY`.

## Examples

### Extract Data

To get specific columns:

```sql
SELECT productCode, SUM(quantityOrdered) AS totalQuantity
FROM orderdetails
GROUP BY productCode;
```

### Filter and Aggregate

To filter and aggregate data:

```sql
SELECT productCode, SUM(quantityOrdered) AS totalQuantity
FROM orderdetails
WHERE quantityOrdered > 100
GROUP BY productCode;
```

## Setup

1. **Database Connection**:
   - Connect to your database using your preferred SQL tool or programming library.

2. **Running Queries**:
   - Execute the provided SQL queries to extract and handle your data.

## Conclusion

This project illustrates fundamental SQL techniques for data extraction and basic analysis. Use the examples to retrieve and analyze data effectively.
