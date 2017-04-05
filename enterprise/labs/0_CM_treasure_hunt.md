
1)What is ubertask optimization?
ubertask is a feature that enables the reuse of a JVM for small tasks.


2)Where in CM is the Kerberos Security Realm value displayed?
Administration -> Settings -> Kerberos

3)Which CDH service(s) host a property for enabling Kerberos authentication?
On Core Hadoop install: Zookeeper, HiveServer2 and HDFS (Authentication for HTTP Web-Consoles)

4)How do you upgrade the CM agents?
Upgrade Cloudera Manager Server fisrt, after you can use an wizard to upgrade agents.

5)Give the tsquery statement used to chart Hue's CPU utilization?
select cpu_system_rate + cpu_user_rate where category=ROLE and serviceName="Hue"

6)Name all the roles that make up the Hive service
HIVESERVER2, HIVEMETASTORE, WEBHCAT, GATEWAY

7)What steps must be completed before integrating Cloudera Manager with Kerberos?
Get or create a Kerberos Principal for the CM server.
