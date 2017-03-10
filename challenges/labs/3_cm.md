>## hdfs dfs -ls /user

```
[hdfs@ip-172-31-17-144 ~]$ hdfs dfs -ls /user
Found 6 items
drwxrwxrwx   - mapred  hadoop             0 2017-03-10 05:07 /user/history
drwxrwxr-t   - hive    hive               0 2017-03-10 05:07 /user/hive
drwxrwxr-x   - hue     hue                0 2017-03-10 05:08 /user/hue
drwxr-xr-x   - neymar  merengues          0 2017-03-10 05:13 /user/neymar
drwxrwxr-x   - oozie   oozie              0 2017-03-10 05:08 /user/oozie
drwxr-xr-x   - ronaldo barca              0 2017-03-10 05:16 /user/ronaldo
```

>## curl Command
```
[hdfs@ip-172-31-17-144 ~]$ curl -u "admin:admin" -i http://35.156.15.161:7180/api/v14/hosts
HTTP/1.1 200 OK
Expires: Thu, 01-Jan-1970 00:00:00 GMT
Set-Cookie: CLOUDERA_MANAGER_SESSIONID=1cnl2z26aky80t59ic4imnt4;Path=/;HttpOnly
Content-Type: application/json
Date: Fri, 10 Mar 2017 10:17:08 GMT
Transfer-Encoding: chunked
Server: Jetty(6.1.26.cloudera.4)

{
  "items" : [ {
    "hostId" : "d1e1ef40-e0ae-43a8-9f3d-85f9fda88ab0",
    "ipAddress" : "172.31.17.144",
    "hostname" : "ip-172-31-17-144.eu-central-1.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-25-25.eu-central-1.compute.internal:7180/cmf/hostRedirect/d1e1ef40-e0ae-43a8-9f3d-85f9fda88ab0",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15331930112
  }, {
    "hostId" : "0c23d387-2290-4a51-9311-87c7a4f6ec5f",
    "ipAddress" : "172.31.21.243",
    "hostname" : "ip-172-31-21-243.eu-central-1.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-25-25.eu-central-1.compute.internal:7180/cmf/hostRedirect/0c23d387-2290-4a51-9311-87c7a4f6ec5f",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15331930112
  }, {
    "hostId" : "087d91cf-7934-4e04-b1c6-5e8a8fec5f3c",
    "ipAddress" : "172.31.23.122",
    "hostname" : "ip-172-31-23-122.eu-central-1.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-25-25.eu-central-1.compute.internal:7180/cmf/hostRedirect/087d91cf-7934-4e04-b1c6-5e8a8fec5f3c",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15331930112
  }, {
    "hostId" : "b2ba882c-3af5-4cdb-8b00-4f4ca4271ca0",
    "ipAddress" : "172.31.23.237",
    "hostname" : "ip-172-31-23-237.eu-central-1.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-25-25.eu-central-1.compute.internal:7180/cmf/hostRedirect/b2ba882c-3af5-4cdb-8b00-4f4ca4271ca0",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15331930112
  }, {
    "hostId" : "a7995f19-2d0c-4c4c-b4f0-92d039a91b7a",
    "ipAddress" : "172.31.25.25",
    "hostname" : "ip-172-31-25-25.eu-central-1.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-25-25.eu-central-1.compute.internal:7180/cmf/hostRedirect/a7995f19-2d0c-4c4c-b4f0-92d039a91b7a",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15331930112
  } ]
}
```
