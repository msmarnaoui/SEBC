>## Teragen 640M output

```
[neymar@ip-172-31-17-144 ~]$ time hadoop jar /opt/cloudera/parcels/CDH-5.10.0-1.cdh5.10.0.p0.41/jars/hadoop-examples.jar teragen -Ddfs.block.size=16777216 6553600  /user/neymar/tgen640m
17/03/10 05:25:45 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-17-144.eu-central-1.compute.internal/172.31.17.144:8032
17/03/10 05:25:46 INFO terasort.TeraGen: Generating 6553600 using 2
17/03/10 05:25:46 INFO mapreduce.JobSubmitter: number of splits:2
17/03/10 05:25:46 INFO Configuration.deprecation: dfs.block.size is deprecated. Instead, use dfs.blocksize
17/03/10 05:25:46 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1489140425772_0003
17/03/10 05:25:46 INFO impl.YarnClientImpl: Submitted application application_1489140425772_0003
17/03/10 05:25:46 INFO mapreduce.Job: The url to track the job: http://ip-172-31-17-144.eu-central-1.compute.internal:8088/proxy/application_1489140425772_0003/
17/03/10 05:25:46 INFO mapreduce.Job: Running job: job_1489140425772_0003
17/03/10 05:25:54 INFO mapreduce.Job: Job job_1489140425772_0003 running in uber mode : false
17/03/10 05:25:54 INFO mapreduce.Job:  map 0% reduce 0%
17/03/10 05:26:07 INFO mapreduce.Job:  map 100% reduce 0%
17/03/10 05:26:07 INFO mapreduce.Job: Job job_1489140425772_0003 completed successfully
17/03/10 05:26:07 INFO mapreduce.Job: Counters: 31
	File System Counters
		FILE: Number of bytes read=0
		FILE: Number of bytes written=249620
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=167
		HDFS: Number of bytes written=655360000
		HDFS: Number of read operations=8
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=4
	Job Counters 
		Launched map tasks=2
		Other local map tasks=2
		Total time spent by all maps in occupied slots (ms)=21272
		Total time spent by all reduces in occupied slots (ms)=0
		Total time spent by all map tasks (ms)=21272
		Total vcore-seconds taken by all map tasks=21272
		Total megabyte-seconds taken by all map tasks=21782528
	Map-Reduce Framework
		Map input records=6553600
		Map output records=6553600
		Input split bytes=167
		Spilled Records=0
		Failed Shuffles=0
		Merged Map outputs=0
		GC time elapsed (ms)=357
		CPU time spent (ms)=17250
		Physical memory (bytes) snapshot=751443968
		Virtual memory (bytes) snapshot=3162378240
		Total committed heap usage (bytes)=866648064
	org.apache.hadoop.examples.terasort.TeraGen$Counters
		CHECKSUM=14071873778075354
	File Input Format Counters 
		Bytes Read=0
	File Output Format Counters 
		Bytes Written=655360000

real	0m24.128s
user	0m5.716s
sys	0m0.271s
```

>## Neymar Directory

```
hdfs dfs -ls /user/neymar/tgen640m
Found 3 items
-rw-r--r--   3 neymar merengues          0 2017-03-10 05:26 /user/neymar/tgen640m/_SUCCESS
-rw-r--r--   3 neymar merengues  327680000 2017-03-10 05:26 /user/neymar/tgen640m/part-m-00000
-rw-r--r--   3 neymar merengues  327680000 2017-03-10 05:26 /user/neymar/tgen640m/part-m-00001

```

>## Neymar Directory Block Count

```
[neymar@ip-172-31-17-144 ~]$ hdfs fsck -blocks /user/neymar/tgen640m
Connecting to namenode via http://ip-172-31-17-144.eu-central-1.compute.internal:50070
FSCK started by neymar (auth:SIMPLE) from /172.31.17.144 for path /user/neymar/tgen640m at Fri Mar 10 05:30:55 EST 2017
...Status: HEALTHY
 Total size:	655360000 B
 Total dirs:	1
 Total files:	3
 Total symlinks:		0
 Total blocks (validated):	40 (avg. block size 16384000 B)
 Minimally replicated blocks:	40 (100.0 %)
 Over-replicated blocks:	0 (0.0 %)
 Under-replicated blocks:	0 (0.0 %)
 Mis-replicated blocks:		0 (0.0 %)
 Default replication factor:	3
 Average block replication:	3.0
 Corrupt blocks:		0
 Missing replicas:		0 (0.0 %)
 Number of data-nodes:		4
 Number of racks:		1
FSCK ended at Fri Mar 10 05:30:55 EST 2017 in 3 milliseconds


The filesystem under path '/user/neymar/tgen640m' is HEALTHY

```


