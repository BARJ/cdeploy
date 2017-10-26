Changelog
=========
2.0 (BARJ/cdeploy Forked from rackerlabs/cdeploy)
---
- Split cql statements by semicolon only if semicolon is at the end of a line
- Store schema migration version as bigint in order to support versions such
   as '201709231354' (yyyymmddhhmm)

1.8
---
- Adds optional port parameter for Cassandra connection

1.7
---
- Properly closes connection to cluster

1.6
---
- Adds configurable default_timeout setting to Cassandra driver session

1.5
---
- Compatibility updates for Cassandra driver 3.0.0 release
- Adds protection against adding duplicate schema migration files
- Adds proper exit code when configuration files are missing
- Integration tests added to tox & Travis CI

1.4
---
- Enables automatic keyspace creation if keyspace isn't found in Cassandra

1.3
---
- Allows migration script filenames to consist entirely of numerals

1.2
---
- Authentication & SSL Cassandra connection options
- Configurable consistency level for all CQL statements

1.1
---
- Python 3 compatibility

1.0
---
- Initial release
