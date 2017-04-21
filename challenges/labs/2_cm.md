[root@ip-172-31-50-139 ~]# ls /etc/yum.repos.d
cloudera-manager.repo           redhat-rhui.repo
redhat.repo                     rhui-load-balancers.conf
redhat-rhui-client-config.repo



root@ip-172-31-50-139 ~]# sudo /usr/share/cmf/schema/scm_prepare_database.sh mysql -h ip-172-31-50-139.ec2.internal -utemp -ptemp --scm-host ip-172-31-50-139.ec2.internal scm scm scm

