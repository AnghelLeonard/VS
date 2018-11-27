| Features | MySQL | PostgreSQL |
|---|---|---|
| **License** | Open source and comercial versions via Oracle | Completely open source |
| **Clients** | GitHub, US Navy, NASA, Tesla, Netflix, WeChat, Facebook, Zendesk, Twitter, Zappos, YouTube, Spotify | Apple, BioPharm, Etsy, IMDB, Macworld, Debian, Fujitsu, Red Hat, Sun Microsystem, Cisco, Skype |
| **Architectural**  | Single process | Multi process |
| **Concurrency** | Multi Thread (default stack size of a thread is at 256KB on 64-bit platforms) | Fork approach. Postgres forks off a child process to establish a connection, it can take up to 10 MB per connection. Pay attention to this if you need a lot of connections, 1000+) |
| **ACID Compliance**  | MySQL is partially ACID compliant. Previous version may not follow ACID. InnoDB and NDB Cluster Storage engines adhere closely to the ACID model. | Fully ACID compliant |
| **SQL Compliance**  | MySQL is partially compliant on some of the versions. PostgreSQL queries are, in most cases, exactly the same as MySQL queries. | Largely SQL compliant. MySQL queries are, in most cases, exactly the same as PostgreSQL queries. |
| **CTEs**  | Starting with MySQL 8 it supports Common Table Expressions , both nonrecursive and recursive.  | Yes |
| **Window Functions**  | Starting with MySQL 8 it supports window functions that, for each row from a query, perform a calculation using rows related to that row.  | Yes |
| **Materialised View**  |  Is missing natively in MySQL, but it could be developed easily with SQL logic. | Yes. To create a materialized view, you use the CREATE MATERIALIZED VIEW. |
| **Temporary Tables** | Yes | Yes |
| **JSON Support** | Yes. Improved in MySQL 8. | Yes |
| **Full-text Search** | Yes | Yes |
| **GIS/SRS** | Geospatial data support is built in. Improved in MySQL 8. | PostgreSQL supports Geospatial data via the PostGIS extension. Easy to use for developers. |
|**Access Methods** | All standards | All standards |
| **Regular expression** | Yes. Before MySQL 8, regular expressions were supported via the Henry Spencer regular expression library. Starting with MySQL 8, regular expression support has been reimplemented using International Components for Unicode (ICU), which provides full Unicode support and is multibyte safe. | Yes. There are three separate approaches to pattern matching provided by PostgreSQL. LIKE operator, the more recent SIMILAR TO operator (added in SQL:1999), and POSIX-style regular expressions. |
| **Extensible Type System** | Some support. For example we can add new functions. | Some support. It is possible to add new types, new functions, new index types, etc. |
| **Connection Management** | Starting with MySQL 8, MySQL Server now permits a TCP/IP port to be configured specifically for administrative connections. |  Does not support a dedicated port. |
| **Security** | In some previous versions, MySQL distribution must be built with SSL support(e.g., MySQL 5.5). In MySQL 8, it supports encrypted connections using the TLSv1, TLSv1.1, and TLSv1.2 protocols. | SSL support |
| **Garbage Collection** | Purge Threads. Runs with dedicated threads inside the separate rollback segment. It doesn't affect the read concurrency in any way. | Auto-vacuum Processes. Is very costly as it works in the main heap area.  Gives you pause at random as the Java GC. |
| **Table Structure** | Clustered Index (preferable to have, lookup by PK trigger a single I/O). Rows are directly embedded inside the B-tree structure of its primary key. For large amount of memory, both clustered and non-clustered are ok. | Heap (non-clustered, lookup by PK trigger at least two I/O, not FK and joins friendly). Regular table structure filled with data rows separately from indexes. For large amount of memory, both clustered and non-clustered are ok. |
|   |   |   |
|   |   |   |
|   |   |   |
|   |   |   |
