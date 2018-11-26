| Features | MySQL | PostgreSQL |
|---|---|---|
| **License** | Open source and comercial versions via Oracle | Completely open source |
| **ACID Compliance**  | Fully ACID compliant  | MySQL is partially ACID compliant. Previous version may not follow ACID. InnoDB and NDB Cluster Storage engines adhere closely to the ACID model. |
| **SQL Compliance**  | Largely SQL compliant. MySQL queries are, in most cases, exactly the same as PostgreSQL queries.  | MySQL is partially compliant on some of the versions. PostgreSQL queries are, in most cases, exactly the same as MySQL queries. |
| **CTEs**  | Starting with MySQL 8 it supports Common Table Expressions , both nonrecursive and recursive.  | Yes |
| **Window Functions**  | Starting with MySQL 8 it supports window functions that, for each row from a query, perform a calculation using rows related to that row.  | Yes |
| **Materialised View**  |  Is missing natively in MySQL, but it could be developed easily with SQL logic. | Yes. To create a materialized view, you use the CREATE MATERIALIZED VIEW. |
|   |   |   |
|   |   |   |
|   |   |   |
|   |   |   |
|   |   |   |
|   |   |   |
