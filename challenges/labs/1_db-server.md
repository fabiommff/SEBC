MariaDB [(none)]> select @@hostname;
+-------------------------------+
| @@hostname                    |
+-------------------------------+
| ip-172-31-50-139.ec2.internal |
+-------------------------------+
1 row in set (0.00 sec)

MariaDB [(none)]> select @@version;
+----------------+
| @@version      |
+----------------+
| 5.5.52-MariaDB |
+----------------+
1 row in set (0.00 sec)

MariaDB [(none)]> show databases;
+--------------------+
| Database           |
+--------------------+
| information_schema |
| amon               |
| hue                |
| metastore          |
| mysql              |
| nav                |
| navms              |
| oozie              |
| performance_schema |
| rman               |
| scm                |
| sentry             |
+--------------------+
12 rows in set (0.00 sec)
