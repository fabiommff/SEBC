[hdfs@ip-172-31-48-240 root]$ hdfs dfs -ls /user
Found 6 items
drwxrwxrwx   - mapred  hadoop             0 2017-04-20 22:00 /user/history
drwxrwxr-t   - hive    hive               0 2017-04-20 22:00 /user/hive
drwxrwxr-x   - hue     hue                0 2017-04-20 22:01 /user/hue
drwxr-xr-x   - neymar  merengues          0 2017-04-20 22:09 /user/neymar
drwxrwxr-x   - oozie   oozie              0 2017-04-20 22:01 /user/oozie
drwxr-xr-x   - ronaldo barca              0 2017-04-20 22:09 /user/ronaldo


[root@ip-172-31-50-139 cloudera-scm-server]# curl -X GET -u "admin:admin" -i http://ip-172-31-50-139.ec2.internal:7180/api/v14/hosts
HTTP/1.1 200 OK
Expires: Thu, 01-Jan-1970 00:00:00 GMT
Set-Cookie: CLOUDERA_MANAGER_SESSIONID=11gjsvb13aulz1f5yogyqp9t69;Path=/;HttpOnly
Content-Type: application/json
Date: Fri, 21 Apr 2017 02:14:36 GMT
Transfer-Encoding: chunked
Server: Jetty(6.1.26.cloudera.4)

{
  "items" : [ {
    "hostId" : "0e41efb4-7a87-4e71-879d-5f815e3ca70a",
    "ipAddress" : "172.31.48.240",
    "hostname" : "ip-172-31-48-240.ec2.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-50-139.ec2.internal:7180/cmf/hostRedirect/0e41efb4-7a87-4e71-879d-5f815e3ca70a",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15331930112
  }, {
    "hostId" : "3c2f4684-dde7-4faf-8296-fa8a24d54b64",
    "ipAddress" : "172.31.50.139",
    "hostname" : "ip-172-31-50-139.ec2.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-50-139.ec2.internal:7180/cmf/hostRedirect/3c2f4684-dde7-4faf-8296-fa8a24d54b64",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15331930112
  }, {
    "hostId" : "596bf0c9-cf72-4aa0-b007-d72d1d4b2234",
    "ipAddress" : "172.31.57.83",
    "hostname" : "ip-172-31-57-83.ec2.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-50-139.ec2.internal:7180/cmf/hostRedirect/596bf0c9-cf72-4aa0-b007-d72d1d4b2234",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15331930112
  }, {
    "hostId" : "979b73d6-4426-42fe-abed-e6d07a952ddf",
    "ipAddress" : "172.31.59.29",
    "hostname" : "ip-172-31-59-29.ec2.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-50-139.ec2.internal:7180/cmf/hostRedirect/979b73d6-4426-42fe-abed-e6d07a952ddf",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15331930112
  }, {
    "hostId" : "6d9ea2a5-d088-45ab-b780-3d3b5ec46b28",
    "ipAddress" : "172.31.63.59",
    "hostname" : "ip-172-31-63-59.ec2.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-50-139.ec2.internal:7180/cmf/hostRedirect/6d9ea2a5-d088-45ab-b780-3d3b5ec46b28",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15331930112
  } ]
}You have new mail in /var/spool/mail/root
