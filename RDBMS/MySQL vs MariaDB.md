| Features | MySQL | MariaDB |
|---|---|---|
| **License** | Open source and comercial versions via Oracle	| Completely open source |
| **Tool/Editing** | MySQL Workbench | Webyog’s SQLYog for Microsoft Windows (MySQL Workbench notes an incompatible server) |
| **Tool/Monitoring** | MySQL Enterprise Monitor | Webyog’s Monyog |
| **Core Replication** | MySQL replication with GTID | MariaDB Server replication, with own GTID, compatible only if MariaDB Server is a slave to MySQL, not vice versa |
| **Core Routing** | MySQL Router (GPLv2) | MariaDB MaxScale (Business Source License) |
| **Core Partitioning** | Standard | Standard, with extra engines like SPIDER/CONNECT that offer varying levels of support |
| **Temporal Log-based rollback** | No | In development for MariaDB Server 10.3 |
| **Temporal System versioned tables** | No | In development for MariaDB Server 10.3 |
| **Official client connectors** | C (libmysqlclient), Java, ODBC, .NET, Node.js, Python, C++, mysqlnd for PHP | C (libmariadbclient), Java, ODBC |
| **Security – Password authentication** | sha256_password (with caching_sha2_password in 8.0) | ed25519 (incompatible with sha256_password) |

https://www.percona.com/blog/2017/11/02/mysql-vs-mariadb-reality-check/
