List the cloud provider you are using (AWS, GCE, Azure, other)
- AWS

List the nodes you are using by IP address and name

172.31.50.139 ip-172-31-50-139.ec2.internal
172.31.57.83  ip-172-31-57-83.ec2.internal
172.31.59.29  ip-172-31-59-29.ec2.internal
172.31.48.240 ip-172-31-48-240.ec2.internal
172.31.63.59  ip-172-31-63-59.ec2.internal

List the Linux release you are using

[root@ip-172-31-50-139 /]# cat /etc/redhat-release
Red Hat Enterprise Linux Server release 7.3 (Maipo)

Demonstrate the disk capacity available on each node is >= 30 GB

[root@ip-172-31-50-139 /]# df .
Filesystem     1K-blocks    Used Available Use% Mounted on
/dev/xvda2      83873772 1334124  82539648   2% /

List the command and output for yum repolist enabled

[root@ip-172-31-50-139 /]# yum repolist enabled
Loaded plugins: amazon-id, rhui-lb, search-disabled-repos
repo id                                          repo name                status
rhui-REGION-client-config-server-7/x86_64        Red Hat Update Infrastru      6
rhui-REGION-rhel-server-releases/7Server/x86_64  Red Hat Enterprise Linux 14,268
rhui-REGION-rhel-server-rh-common/7Server/x86_64 Red Hat Enterprise Linux    225
repolist: 14,499



Reproduced for all nodes:

[root@ip-172-31-50-139 /]# useradd -u 2010 neymar
useradd -u 2016 ronaldo
groupadd barca
groupadd merengues
usermod -a -G barca ronaldo
usermod -a -G merengues neymar
cat /etc/passwd | grep neymar
cat /etc/passwd | grep ronaldo
[root@ip-172-31-50-139 /]# useradd -u 2016 ronaldo
[root@ip-172-31-50-139 /]# groupadd barca
[root@ip-172-31-50-139 /]# groupadd merengues
cat /etc/group | grep barca
[root@ip-172-31-50-139 /]# usermod -a -G barca ronaldo
[root@ip-172-31-50-139 /]# usermod -a -G merengues neymar
[root@ip-172-31-50-139 /]# cat /etc/passwd | grep neymar
neymar:x:2010:2010::/home/neymar:/bin/bash
[root@ip-172-31-50-139 /]# cat /etc/passwd | grep ronaldo
ronaldo:x:2016:2016::/home/ronaldo:/bin/bash
[root@ip-172-31-50-139 /]# cat /etc/group | grep barca
barca:x:2017:ronaldo
[root@ip-172-31-50-139 /]# cat /etc/group | grep merengues
merengues:x:2018:neymar

