#Latest API 
 curl -u "msmarnaoui:cloudera" -i   http://35.167.64.53:7180/api/version
<strong> 15 </strong>

#CM version
curl -u "msmarnaoui:cloudera" -i   http://35.167.64.53:7180/api/v2/cm/version

```json
{
  "version" : "5.10.0",
  "buildUser" : "jenkins",
  "buildTimestamp" : "20170120-1037",
  "gitHash" : "aa0b5cd5eceaefe2f971c13ab657020d96bb842a",
  "snapshot" : false
}
```

# CM users

curl -u "msmarnaoui:cloudera" -i   http://35.167.64.53:7180/api/v2/users
```json
{
  "items" : [ {
    "name" : "admin",
    "roles" : [ "ROLE_LIMITED" ]
  }, {
    "name" : "minotaur",
    "roles" : [ "ROLE_CONFIGURATOR" ]
  }, {
    "name" : "msmarnaoui",
    "roles" : [ "ROLE_ADMIN" ]
  } ]
}
```

# Report the database server in use by CM

curl -u "msmarnaoui:cloudera" -i http://35.167.64.53:7180/api/v2/cm/service/roles/mgmt-REPORTSMANAGER-7be275fc706044f09590a812053baca2/config
```json
{
  "items" : [ {
    "name" : "headlamp_database_host",
    "value" : "ec2-35-167-64-53.us-west-2.compute.amazonaws.com"
  }, {
    "name" : "headlamp_database_name",
    "value" : "rman"
  }, {
    "name" : "headlamp_database_password",
    "value" : "rman"
  }, {
    "name" : "headlamp_database_user",
    "value" : "rman"
  }, {
    "name" : "headlamp_heapsize",
    "value" : "593494016"
  } ]
}
```
