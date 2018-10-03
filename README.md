# docker-aerospike

```
$ aql
Aerospike Query Client
Version 3.13.0.1
C Client Version 4.1.6
Copyright 2012-2016 Aerospike. All rights reserved.
aql> insert into test.sample (PK, name, price, description) values (1, 'Ringo', 100, 'from Aomori')
OK, 1 record affected.

aql> show namespaces
+------------+
| namespaces |
+------------+
| "test"     |
+------------+
1 row in set (0.001 secs)
OK

aql> show sets
+------------------+--------+----------------+---------+-------------------+----------+-------------------+--------------+------------+
| disable-eviction | ns     | set-enable-xdr | objects | stop-writes-count | set      | memory_data_bytes | truncate_lut | tombstones |
+------------------+--------+----------------+---------+-------------------+----------+-------------------+--------------+------------+
| "false"          | "test" | "use-default"  | 1       | 0                 | "sample" | 64                | 0            | 0          |
+------------------+--------+----------------+---------+-------------------+----------+-------------------+--------------+------------+
1 row in set (0.000 secs)
OK

aql> select * from test.sample
+---------+-------+---------------+
| name    | price | description   |
+---------+-------+---------------+
| "Ringo" | 100   | "from Aomori" |
+---------+-------+---------------+
1 row in set (0.165 secs)

```
