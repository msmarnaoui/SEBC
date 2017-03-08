<strong> What is ubertask optimization? </strong>
Uber jobs are jobs that are executed within the MapReduce ApplicationMaster to avoid the overhead of launching and communicate with remote containers.

If you have a small dataset or you want to run MapReduce on small amount of data, Uber configuration will help you out, by reducing additional time that MapReduce normally spends in mapper and reducers phase.

<strong>Which CDH service(s) host a property for enabling Kerberos authentication? </strong>
we could enable kerberos for the cluster from the cloudera manager admin console.

<strong> How do you upgrade the CM agents? </strong>
After upgrading CM server, we could upgrade the agents using a upgrade wizard from the Admin console or manually install the CM agent packages 
<strong> Give the tsquery statement used to chart Hue's CPU utilization? </strong>
select cpu_user_rate where roleType=HUE_SERVER

<strong> Name all the roles that make up the Hive service </strong>
Gateway
Hive Metastore Server
HiveServer


<strong> What steps must be completed before integrating Cloudera Manager with Kerberos? </strong>
* Ensure we have secured communication between the CM Server and Agents 
* Install a KDC and Realm
* Install Kerberos client packages on all cluster hosts 
* Install Kerberos client packages hosts that will be used to access the cluster 
* Install the Java Cryptography Extension (JCE) Unlimited Strength Jurisdiction Policy File on all cluster and Hadoop user hosts
* Create a Kerberos Principal for the Cloudera Manager Server

