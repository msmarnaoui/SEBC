# Teragen 500 Mo File
hadoop jar /opt/cloudera/parcels/CDH-5.10.0-1.cdh5.10.0.p0.41/jars/hadoop-examples.jar teragen 524288000  /user/msmarnaoui/msmarnaoui


# Teragen 10 Go File
time hadoop jar /opt/cloudera/parcels/CDH-5.10.0-1.cdh5.10.0.p0.41/jars/hadoop-examples.jar teragen -Ddfs.block.size=33554432 -Dmapred.map.tasks=4  100000000  /user/msmarnaoui/msmarnaoui_10Go

'''Time outout: 
real	2m33.782s
user	0m6.235s
sys	0m0.307s
'''


# terasort 
time hadoop jar /opt/cloudera/parcels/CDH-5.10.0-1.cdh5.10.0.p0.41/jars/hadoop-examples.jar terasort /user/msmarnaoui/msmarnaoui_10Go /user/msmarnaoui/terasort_10g 

'''Time Output:
real	7m28.797s
user	0m9.542s
sys	0m0.376s

'''
