**/etc/yum.repo.d**
```
[root@ip-172-31-25-25 ~]# ls /etc/yum.repos.d
cloudera-manager.repo  mysql-community-source.repo  redhat-rhui-client-config.repo  rhui-load-balancers.conf
mysql-community.repo   redhat.repo                  redhat-rhui.repo

```

***scm_prepare_database.sh***
```
/usr/share/cmf/schema/scm_prepare_database.sh mysql -f -h ip-172-31-23-122.eu-central-1.compute.internal -utemp -ptemp --scm-host ip-172-31-25-25.eu-central-1.compute.internala scm scm admin
```

