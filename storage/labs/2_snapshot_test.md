su -msmarnaoui

* hdfs dfs -mkdir /user/msmarnaoui/precuous

* hdfs dfs -put SEBC.zip /user/msmarnaoui/precious/


su - hdfs

* hdfs dfsadmin -allowSnapshot /user/msmarnaoui/precuous

Allowing snaphot on /user/msmarnaoui/precuous succeeded


su - msmarnaoui

* hdfs dfs -createSnapshot /user/msmarnaoui/precuous sebc-hdfs-test

Created snapshot /user/msmarnaoui/precuous/.snapshot/sebc-hdfs-test

