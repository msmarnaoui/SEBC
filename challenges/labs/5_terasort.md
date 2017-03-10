>## Terasort Output

```
[neymar@ip-172-31-25-25 ~]$ time hadoop jar /opt/cloudera/parcels/CDH-5.10.0-1.cdh5.10.0.p0.41/jars/hadoop-examples.jar terasort /user/neymar/tgen640m /user/neymar/tsort640m
17/03/10 06:01:01 INFO terasort.TeraSort: starting
17/03/10 06:01:03 INFO hdfs.DFSClient: Created token for neymar: HDFS_DELEGATION_TOKEN owner=neymar@MSMARNAOUI.ES, renewer=yarn, realUser=, issueDate=1489143662976, maxDate=1489748462976, sequenceNumber=1, masterKeyId=2 on 172.31.17.144:8020
17/03/10 06:01:03 INFO security.TokenCache: Got dt for hdfs://ip-172-31-17-144.eu-central-1.compute.internal:8020; Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.17.144:8020, Ident: (token for neymar: HDFS_DELEGATION_TOKEN owner=neymar@MSMARNAOUI.ES, renewer=yarn, realUser=, issueDate=1489143662976, maxDate=1489748462976, sequenceNumber=1, masterKeyId=2)
17/03/10 06:01:03 INFO input.FileInputFormat: Total input paths to process : 2
Spent 310ms computing base-splits.
Spent 2ms computing TeraScheduler splits.
Computing input splits took 313ms
Sampling 10 splits of 40
Making 8 from 100000 sampled records
Computing parititions took 821ms
Spent 1137ms computing partitions.
17/03/10 06:01:04 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-17-144.eu-central-1.compute.internal/172.31.17.144:8032
17/03/10 06:01:04 INFO mapreduce.JobSubmitter: number of splits:40
17/03/10 06:01:04 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1489143453431_0001
17/03/10 06:01:04 INFO mapreduce.JobSubmitter: Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.17.144:8020, Ident: (token for neymar: HDFS_DELEGATION_TOKEN owner=neymar@MSMARNAOUI.ES, renewer=yarn, realUser=, issueDate=1489143662976, maxDate=1489748462976, sequenceNumber=1, masterKeyId=2)
17/03/10 06:01:05 INFO impl.YarnClientImpl: Submitted application application_1489143453431_0001
17/03/10 06:01:05 INFO mapreduce.Job: The url to track the job: http://ip-172-31-17-144.eu-central-1.compute.internal:8088/proxy/application_1489143453431_0001/
17/03/10 06:01:05 INFO mapreduce.Job: Running job: job_1489143453431_0001
17/03/10 06:01:16 INFO mapreduce.Job: Job job_1489143453431_0001 running in uber mode : false
17/03/10 06:01:16 INFO mapreduce.Job:  map 0% reduce 0%
17/03/10 06:01:25 INFO mapreduce.Job:  map 3% reduce 0%
17/03/10 06:01:26 INFO mapreduce.Job:  map 8% reduce 0%
17/03/10 06:01:34 INFO mapreduce.Job:  map 13% reduce 0%
17/03/10 06:01:35 INFO mapreduce.Job:  map 35% reduce 0%
17/03/10 06:01:36 INFO mapreduce.Job:  map 45% reduce 0%
17/03/10 06:01:44 INFO mapreduce.Job:  map 50% reduce 0%
17/03/10 06:01:45 INFO mapreduce.Job:  map 52% reduce 0%
17/03/10 06:01:48 INFO mapreduce.Job:  map 73% reduce 0%
17/03/10 06:01:49 INFO mapreduce.Job:  map 82% reduce 0%
17/03/10 06:01:55 INFO mapreduce.Job:  map 90% reduce 0%
17/03/10 06:01:59 INFO mapreduce.Job:  map 93% reduce 0%
17/03/10 06:02:00 INFO mapreduce.Job:  map 100% reduce 0%
17/03/10 06:02:06 INFO mapreduce.Job:  map 100% reduce 13%
17/03/10 06:02:07 INFO mapreduce.Job:  map 100% reduce 100%
17/03/10 06:02:08 INFO mapreduce.Job: Job job_1489143453431_0001 completed successfully
17/03/10 06:02:09 INFO mapreduce.Job: Counters: 49
	File System Counters
		FILE: Number of bytes read=288339686
		FILE: Number of bytes written=578749394
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=655366280
		HDFS: Number of bytes written=655360000
		HDFS: Number of read operations=144
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=16
	Job Counters 
		Launched map tasks=40
		Launched reduce tasks=8
		Data-local map tasks=40
		Total time spent by all maps in occupied slots (ms)=499238
		Total time spent by all reduces in occupied slots (ms)=121938
		Total time spent by all map tasks (ms)=499238
		Total time spent by all reduce tasks (ms)=121938
		Total vcore-seconds taken by all map tasks=499238
		Total vcore-seconds taken by all reduce tasks=121938
		Total megabyte-seconds taken by all map tasks=511219712
		Total megabyte-seconds taken by all reduce tasks=124864512
	Map-Reduce Framework
		Map input records=6553600
		Map output records=6553600
		Map output bytes=668467200
		Map output materialized bytes=284310654
		Input split bytes=6280
		Combine input records=0
		Combine output records=0
		Reduce input groups=6553600
		Reduce shuffle bytes=284310654
		Reduce input records=6553600
		Reduce output records=6553600
		Spilled Records=13107200
		Shuffled Maps =320
		Failed Shuffles=0
		Merged Map outputs=320
		GC time elapsed (ms)=7083
		CPU time spent (ms)=178480
		Physical memory (bytes) snapshot=22329749504
		Virtual memory (bytes) snapshot=75747061760
		Total committed heap usage (bytes)=25665470464
	Shuffle Errors
		BAD_ID=0
		CONNECTION=0
		IO_ERROR=0
		WRONG_LENGTH=0
		WRONG_MAP=0
		WRONG_REDUCE=0
	File Input Format Counters 
		Bytes Read=655360000
	File Output Format Counters 
		Bytes Written=655360000
17/03/10 06:02:09 INFO terasort.TeraSort: done

real	1m8.802s
user	0m7.951s
sys	0m0.345s

```

