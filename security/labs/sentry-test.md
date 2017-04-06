[root@ip-172-31-60-231 ~]# kinit fabiommff
Password for fabiommff@EC2.INTERNAL:
[root@ip-172-31-60-231 ~]# beeline
Beeline version 1.1.0-cdh5.10.1 by Apache Hive
beeline> !connect jdbc:hive2://ip-172-31-48-155.ec2.internal:10000/default;princ
ipal=hive/ip-172-31-48-155.ec2.internal@EC2.INTERNAL
Connecting to jdbc:hive2://ip-172-31-48-155.ec2.internal:10000/default;principal
=hive/ip-172-31-48-155.ec2.internal@EC2.INTERNAL
Connected to: Apache Hive (version 1.1.0-cdh5.10.1)
Driver: Hive JDBC (version 1.1.0-cdh5.10.1)
Transaction isolation: TRANSACTION_REPEATABLE_READ
0: jdbc:hive2://ip-172-31-48-155.ec2.internal> SHOW TABLES;
INFO  : Compiling command(queryId=hive_20170406151717_52628a7d-aabc-4efc-99a4-bf525a82aa93): SHOW TABLES
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20170406151717_52628a7d-aabc-4efc-99a4-bf525a82aa93); Time taken: 0.706 seconds
INFO  : Executing command(queryId=hive_20170406151717_52628a7d-aabc-4efc-99a4-bf525a82aa93): SHOW TABLES
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170406151717_52628a7d-aabc-4efc-99a4-bf525a82aa93); Time taken: 0.255 seconds
INFO  : OK
+-----------+--+
| tab_name  |
+-----------+--+
+-----------+--+
No rows selected (2.324 seconds)

0: jdbc:hive2://ip-172-31-48-155.ec2.internal> show tables;
INFO  : Compiling command(queryId=hive_20170406160808_a7d2113d-d506-4248-a097-7b2a25b79e4c): show tables
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20170406160808_a7d2113d-d506-4248-a097-7b2a25b79e4c); Time taken: 0.056 seconds
INFO  : Executing command(queryId=hive_20170406160808_a7d2113d-d506-4248-a097-7b2a25b79e4c): show tables
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170406160808_a7d2113d-d506-4248-a097-7b2a25b79e4c); Time taken: 0.102 seconds
INFO  : OK
+------------+--+
|  tab_name  |
+------------+--+
| customers  |
| sample_07  |
| sample_08  |
| web_logs   |
+------------+--+
4 rows selected (0.181 seconds)

[root@ip-172-31-60-231 ~]# kinit george
Password for george@EC2.INTERNAL:
[root@ip-172-31-60-231 ~]# beeline
Beeline version 1.1.0-cdh5.10.1 by Apache Hive
beeline> SHOW TABLES;
No current connection
beeline> !connect jdbc:hive2://ip-172-31-48-155.ec2.internal:10000/default;principal=hive/ip-172-31-48-155.ec2.internal@EC2.INTERNAL
scan complete in 2ms
Connecting to jdbc:hive2://ip-172-31-48-155.ec2.internal:10000/default;principal=hive/ip-172-31-48-155.ec2.internal@EC2.INTERNAL
Connected to: Apache Hive (version 1.1.0-cdh5.10.1)
Driver: Hive JDBC (version 1.1.0-cdh5.10.1)
Transaction isolation: TRANSACTION_REPEATABLE_READ
0: jdbc:hive2://ip-172-31-48-155.ec2.internal> show tables;
INFO  : Compiling command(queryId=hive_20170406162626_4c46172f-d45d-4dd0-9e98-540ce0f72156): show tables
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20170406162626_4c46172f-d45d-4dd0-9e98-540ce0f72156); Time taken: 0.064 seconds
INFO  : Executing command(queryId=hive_20170406162626_4c46172f-d45d-4dd0-9e98-540ce0f72156): show tables
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170406162626_4c46172f-d45d-4dd0-9e98-540ce0f72156); Time taken: 0.123 seconds
INFO  : OK
+------------+--+
|  tab_name  |
+------------+--+
| customers  |
| sample_07  |
| sample_08  |
| web_logs   |
+------------+--+
4 rows selected (0.282 seconds)
[root@ip-172-31-60-231 ~]# kinit ferdinand
Password for ferdinand@EC2.INTERNAL:
[root@ip-172-31-60-231 ~]# beeline
Beeline version 1.1.0-cdh5.10.1 by Apache Hive
beeline> !connect jdbc:hive2://ip-172-31-48-155.ec2.internal:10000/default;principal=hive/ip-172-31-48-155.ec2.internal@EC2.INTERNAL
scan complete in 2ms
Connecting to jdbc:hive2://ip-172-31-48-155.ec2.internal:10000/default;principal=hive/ip-172-31-48-155.ec2.internal@EC2.INTERNAL
Connected to: Apache Hive (version 1.1.0-cdh5.10.1)
Driver: Hive JDBC (version 1.1.0-cdh5.10.1)
Transaction isolation: TRANSACTION_REPEATABLE_READ
0: jdbc:hive2://ip-172-31-48-155.ec2.internal> show tables;
INFO  : Compiling command(queryId=hive_20170406163131_94870d71-992b-41c5-93e4-4b512848c39f): show tables
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20170406163131_94870d71-992b-41c5-93e4-4b512848c39f); Time taken: 0.061 seconds
INFO  : Executing command(queryId=hive_20170406163131_94870d71-992b-41c5-93e4-4b512848c39f): show tables
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170406163131_94870d71-992b-41c5-93e4-4b512848c39f); Time taken: 0.126 seconds
INFO  : OK
+------------+--+
|  tab_name  |
+------------+--+
| sample_07  |
+------------+--+
1 row selected (0.275 seconds)
