# fsck on my backup cluster of mustafatok file

[hdfs@ip-172-31-7-46 ~]$ hdfs fsck /user/backup/mustafatok/teragen_data -files -blocks
Connecting to namenode via http://ip-172-31-7-46.us-west-2.compute.internal:50070

FSCK started by hdfs (auth:SIMPLE) from /172.31.7.46 for path /user/backup/mustafatok/teragen_data at Wed Mar 08 15:56:21 CET 2017

/user/backup/mustafatok/teragen_data <dir>

/user/backup/mustafatok/teragen_data/_SUCCESS 0 bytes, 0 block(s):  OK

/user/backup/mustafatok/teragen_data/part-m-00000 262144000 bytes, 2 block(s):  OK

0. BP-535643669-172.31.2.148-1488895385476:blk_1073746767_5943 len=134217728 Live_repl=3

1. BP-535643669-172.31.2.148-1488895385476:blk_1073746769_5945 len=127926272 Live_repl=3

/user/backup/mustafatok/teragen_data/part-m-00001 262144000 bytes, 2 block(s):  OK

0. BP-535643669-172.31.2.148-1488895385476:blk_1073746763_5939 len=134217728 Live_repl=3

1. BP-535643669-172.31.2.148-1488895385476:blk_1073746768_5944 len=127926272 Live_repl=3

Status: HEALTHY

 Total size:	524288000 B

 Total dirs:	1

 Total files:	3

 Total symlinks:		0

 Total blocks (validated):	4 (avg. block size 131072000 B)

 Minimally replicated blocks:	4 (100.0 %)

 Over-replicated blocks:	0 (0.0 %)

 Under-replicated blocks:	0 (0.0 %)

 Mis-replicated blocks:		0 (0.0 %)

 Default replication factor:	3

 Average block replication:	3.0

 Corrupt blocks:		0

 Missing replicas:		0 (0.0 %)

 Number of data-nodes:		4

 Number of racks:		1

FSCK ended at Wed Mar 08 15:56:21 CET 2017 in 2 milliseconds

The filesystem under path '/user/backup/mustafatok/teragen_data' is HEALTHY


