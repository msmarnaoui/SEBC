# Stop Hive


curl -X POST -u msmarnaoui:cloudera 'http://35.167.64.53:7180/api/v1/clusters/MSMARNAOUI_Cluster/services/hive/commands/stop'
```json 
{
  "id" : 1133,
  "name" : "Stop",
  "startTime" : "2017-03-08T11:22:59.794Z",
  "active" : true,
  "serviceRef" : {
    "clusterName" : "cluster",
    "serviceName" : "hive"
  }
}
```

# Start Hive

curl -X POST -u msmarnaoui:cloudera 'http://35.167.64.53:7180/api/v1/clusters/MSMARNAOUI_Cluster/services/hive/commands/start'
```json
{
  "id" : 1137,
  "name" : "Start",
  "startTime" : "2017-03-08T11:26:34.610Z",
  "active" : true,
  "serviceRef" : {
    "clusterName" : "cluster",
    "serviceName" : "hive"
  }
}
```

# Check Hive 

curl -u msmarnaoui:cloudera 'http://35.167.64.53:7180/api/v1/clusters/MSMARNAOUI_Cluster/services/hive'

```json
{
  "name" : "hive",
  "type" : "HIVE",
  "clusterRef" : {
    "clusterName" : "cluster"
  },
  "serviceUrl" : "http://ip-172-31-7-46.us-west-2.compute.internal:7180/cmf/serviceRedirect/hive",
  "serviceState" : "STARTED",
  "healthSummary" : "GOOD",
  "healthChecks" : [ {
    "name" : "HIVE_HIVEMETASTORES_HEALTHY",
    "summary" : "GOOD"
  }, {
    "name" : "HIVE_HIVESERVER2S_HEALTHY",
    "summary" : "GOOD"
  } ],
  "configStale" : false
}
```
