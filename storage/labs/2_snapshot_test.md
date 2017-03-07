[msmarnaoui@ip-172-31-10-236 ~]$ hdfs dfs -mkdir /user/msmarnaoui/precuous

[msmarnaoui@ip-172-31-10-236 ~]$ exit

logout

You have new mail in /var/spool/mail/root

[root@ip-172-31-10-236 ~]# su - hdfs
Last login: Tue Mar  7 18:17:12 CET 2017 on pts/0

-bash-4.2$ hdfs dfsadmin -allowSnapshot /user/msmarnaoui/precuous

Allowing snaphot on /user/msmarnaoui/precuous succeeded

-bash-4.2$ exit
logout

[root@ip-172-31-10-236 ~]# su - msmarnaoui

Last login: Tue Mar  7 18:19:00 CET 2017 on pts/0

[msmarnaoui@ip-172-31-10-236 ~]$ hdfs dfs -createSnapshot /user/msmarnaoui/precuous sebc-hdfs-test

Created snapshot /user/msmarnaoui/precuous/.snapshot/sebc-hdfs-test

