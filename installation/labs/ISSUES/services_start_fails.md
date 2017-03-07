
<strong> Problem Description </strong>
hdfs, yarn, zookeeper , oozie are not able to start after installation,

<strong>Troubleshooting</strong>
According to log files of each service, the above services were not able to access their respective folders under /var/lib/, permission denied

these folders were owned by hadoop and no access at all was allowed: D --- --- --- root root ....

it's a little bit strange because this problem occurs only on 4 nodes but not on the CM node from which installation is launched.

<strong>Solution</strong>
a quick fix is to chown and chmod those folders

* chown hdfs:hdfs -R /var/lib/hadoop-hdfs

* chown yarn:yarn -R /var/lib/hadoop-yarn

* chown kms:kms -R /var/lib/hadoop-kms

* chown mapred:mapred -R /var/lib/hadoop-mapreduce

* chown -R httpfs:httpfs /var/lib/hadoop-httpfs

* chmod -R 755 /var/lib/hadoop-*

Service were able to start after this.





