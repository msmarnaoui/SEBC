```json
HTTP/1.1 200 OK
Expires: Thu, 01-Jan-1970 00:00:00 GMT
Set-Cookie: CLOUDERA_MANAGER_SESSIONID=1l3rtl9we6e7je0lt6ldqlj3o;Path=/;HttpOnly
Content-Type: application/json
Date: Wed, 08 Mar 2017 11:06:36 GMT
Transfer-Encoding: chunked
Server: Jetty(6.1.26.cloudera.4)

{
  "timestamp" : "2017-03-08T11:06:36.461Z",
  "clusters" : [ {
    "name" : "MSMARNAOUI_Cluster",
    "version" : "CDH5",
    "services" : [ {
      "name" : "zookeeper",
      "type" : "ZOOKEEPER",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "SERVER",
          "items" : [ {
            "name" : "dataDir",
            "value" : "/home/zookeeper"
          }, {
            "name" : "dataLogDir",
            "value" : "/home/zookeeper"
          }, {
            "name" : "zookeeper_server_java_heapsize",
            "value" : "593494016"
          } ]
        } ],
        "items" : [ ]
      },
      "roles" : [ {
        "name" : "zookeeper-SERVER-49730cc9b75563a071086a68836a0f68",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "34dc2f98-44e4-48bb-9b9c-d2a3283e0a56"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "1yzdszm78h7oytbila74we36b"
          }, {
            "name" : "serverId",
            "value" : "3"
          } ]
        }
      }, {
        "name" : "zookeeper-SERVER-4c7d33ab85eb65a18f81f29a049724b0",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "2e882be2-3f62-4bd2-a3d1-a4e52ad18ff1"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "5m979z0ck9zqt8olol3ioe0we"
          }, {
            "name" : "serverId",
            "value" : "2"
          } ]
        }
      }, {
        "name" : "zookeeper-SERVER-7be275fc706044f09590a812053baca2",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "b24c7526-57ef-4d95-9146-6c38e889e9bb"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "9qcuxye85l7atxtnoxh6fbkro"
          }, {
            "name" : "serverId",
            "value" : "1"
          } ]
        }
      } ],
      "displayName" : "ZooKeeper"
    }, {
      "name" : "hdfs",
      "type" : "HDFS",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "DATANODE",
          "items" : [ {
            "name" : "datanode_java_heapsize",
            "value" : "1073741824"
          }, {
            "name" : "dfs_data_dir_list",
            "value" : "/dfs/dn"
          }, {
            "name" : "dfs_datanode_du_reserved",
            "value" : "5367448780"
          }, {
            "name" : "dfs_datanode_max_locked_memory",
            "value" : "4294967296"
          }, {
            "name" : "rm_cpu_shares",
            "value" : "200"
          }, {
            "name" : "rm_io_weight",
            "value" : "100"
          } ]
        }, {
          "roleType" : "GATEWAY",
          "items" : [ {
            "name" : "dfs_client_use_trash",
            "value" : "true"
          } ]
        }, {
          "roleType" : "JOURNALNODE",
          "items" : [ {
            "name" : "dfs_journalnode_edits_dir",
            "value" : "/dfs/journalnodes"
          } ]
        }, {
          "roleType" : "NAMENODE",
          "items" : [ {
            "name" : "dfs_name_dir_list",
            "value" : "/dfs/nn"
          }, {
            "name" : "dfs_namenode_servicerpc_address",
            "value" : "8022"
          } ]
        }, {
          "roleType" : "SECONDARYNAMENODE",
          "items" : [ {
            "name" : "fs_checkpoint_dir_list",
            "value" : "/dfs/snn"
          } ]
        } ],
        "items" : [ {
          "name" : "dfs_ha_fencing_cloudera_manager_secret_key",
          "value" : "bJiBIZMcajfS7jv9TxRk36vIR85ozl"
        }, {
          "name" : "dfs_ha_fencing_methods",
          "value" : "shell(true)"
        }, {
          "name" : "fc_authorization_secret_key",
          "value" : "L5xQUEFQqIhKlk22VefHwPBXefxvbB"
        }, {
          "name" : "http_auth_signature_secret",
          "value" : "zpUUcJRj8RHaQOOWHrhMkaNi0yZzOh"
        }, {
          "name" : "rm_dirty",
          "value" : "false"
        }, {
          "name" : "rm_last_allocation_percentage",
          "value" : "10"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hdfs-BALANCER-7be275fc706044f09590a812053baca2",
        "type" : "BALANCER",
        "hostRef" : {
          "hostId" : "b24c7526-57ef-4d95-9146-6c38e889e9bb"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hdfs-DATANODE-49730cc9b75563a071086a68836a0f68",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "34dc2f98-44e4-48bb-9b9c-d2a3283e0a56"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "6dn79ule6gj5sro3e5ymlyikl"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-4c7d33ab85eb65a18f81f29a049724b0",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "2e882be2-3f62-4bd2-a3d1-a4e52ad18ff1"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "glyimohk8n1t5q1lsvchtazx"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-62df31e1595c36f8802fabd4c07f0faf",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "31710729-d236-402a-9c76-795406c8d203"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "dc9xl521vvnkdlmxrv4ufkso0"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-8953e23ba3c26181b46a7f4e7779f088",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "61e435e3-259c-45ed-b9af-81fa75be7f17"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "9pt6vcfjj9oplhcy6pzp7tixi"
          } ]
        }
      }, {
        "name" : "hdfs-FAILOVERCONTROLLER-62df31e1595c36f8802fabd4c07f0faf",
        "type" : "FAILOVERCONTROLLER",
        "hostRef" : {
          "hostId" : "31710729-d236-402a-9c76-795406c8d203"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "1bvmkg8mk7w393os7mxa6ska6"
          } ]
        }
      }, {
        "name" : "hdfs-FAILOVERCONTROLLER-8953e23ba3c26181b46a7f4e7779f088",
        "type" : "FAILOVERCONTROLLER",
        "hostRef" : {
          "hostId" : "61e435e3-259c-45ed-b9af-81fa75be7f17"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "brv630q2mf4b3g9uf9xhg787c"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-49730cc9b75563a071086a68836a0f68",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "34dc2f98-44e4-48bb-9b9c-d2a3283e0a56"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "75jjtcmhmaoa12zjz62lngs58"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-62df31e1595c36f8802fabd4c07f0faf",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "31710729-d236-402a-9c76-795406c8d203"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "ctd17pgq5kk8k1mia5pesionj"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-8953e23ba3c26181b46a7f4e7779f088",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "61e435e3-259c-45ed-b9af-81fa75be7f17"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "1fwr649q4treox901af5zgje3"
          } ]
        }
      }, {
        "name" : "hdfs-NAMENODE-62df31e1595c36f8802fabd4c07f0faf",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "31710729-d236-402a-9c76-795406c8d203"
        },
        "config" : {
          "items" : [ {
            "name" : "autofailover_enabled",
            "value" : "true"
          }, {
            "name" : "dfs_federation_namenode_nameservice",
            "value" : "HDFS-HA"
          }, {
            "name" : "dfs_namenode_quorum_journal_name",
            "value" : "HDFS-HA"
          }, {
            "name" : "namenode_id",
            "value" : "89"
          }, {
            "name" : "role_jceks_password",
            "value" : "bqps24frxiliw60wuip4asnu1"
          } ]
        }
      }, {
        "name" : "hdfs-NAMENODE-8953e23ba3c26181b46a7f4e7779f088",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "61e435e3-259c-45ed-b9af-81fa75be7f17"
        },
        "config" : {
          "items" : [ {
            "name" : "autofailover_enabled",
            "value" : "true"
          }, {
            "name" : "dfs_federation_namenode_nameservice",
            "value" : "HDFS-HA"
          }, {
            "name" : "dfs_namenode_quorum_journal_name",
            "value" : "HDFS-HA"
          }, {
            "name" : "namenode_id",
            "value" : "128"
          }, {
            "name" : "role_jceks_password",
            "value" : "1hac4wisnrdwy5sq2vgpirjm5"
          } ]
        }
      } ],
      "displayName" : "HDFS"
    }, {
      "name" : "yarn",
      "type" : "YARN",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "GATEWAY",
          "items" : [ {
            "name" : "mapred_reduce_tasks",
            "value" : "8"
          }, {
            "name" : "mapred_submit_replication",
            "value" : "2"
          } ]
        }, {
          "roleType" : "NODEMANAGER",
          "items" : [ {
            "name" : "yarn_nodemanager_heartbeat_interval_ms",
            "value" : "100"
          }, {
            "name" : "yarn_nodemanager_local_dirs",
            "value" : "/yarn/nm"
          }, {
            "name" : "yarn_nodemanager_log_dirs",
            "value" : "/yarn/container-logs"
          }, {
            "name" : "yarn_nodemanager_resource_cpu_vcores",
            "value" : "4"
          }, {
            "name" : "yarn_nodemanager_resource_memory_mb",
            "value" : "4138"
          } ]
        }, {
          "roleType" : "RESOURCEMANAGER",
          "items" : [ {
            "name" : "yarn_scheduler_maximum_allocation_mb",
            "value" : "4138"
          }, {
            "name" : "yarn_scheduler_maximum_allocation_vcores",
            "value" : "3"
          } ]
        } ],
        "items" : [ {
          "name" : "hdfs_service",
          "value" : "hdfs"
        }, {
          "name" : "rm_dirty",
          "value" : "false"
        }, {
          "name" : "rm_last_allocation_percentage",
          "value" : "90"
        }, {
          "name" : "yarn_service_cgroups",
          "value" : "false"
        }, {
          "name" : "yarn_service_lce_always",
          "value" : "false"
        }, {
          "name" : "zk_authorization_secret_key",
          "value" : "1ir924uigFFIjjdWoAOPSMGLLJioJo"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "yarn-JOBHISTORY-7be275fc706044f09590a812053baca2",
        "type" : "JOBHISTORY",
        "hostRef" : {
          "hostId" : "b24c7526-57ef-4d95-9146-6c38e889e9bb"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "7u35lsnjotp5hcd19se7vrya7"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-49730cc9b75563a071086a68836a0f68",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "34dc2f98-44e4-48bb-9b9c-d2a3283e0a56"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "9omrzsntyok4p0iev4mz42jw4"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-4c7d33ab85eb65a18f81f29a049724b0",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "2e882be2-3f62-4bd2-a3d1-a4e52ad18ff1"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "2msuk1gba9sgencodtinxu5wp"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-62df31e1595c36f8802fabd4c07f0faf",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "31710729-d236-402a-9c76-795406c8d203"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "5x81qpsevg9teyjua0vf8ivbk"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-8953e23ba3c26181b46a7f4e7779f088",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "61e435e3-259c-45ed-b9af-81fa75be7f17"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "bpwzj0d4trz6ijhlrwdft8bwl"
          } ]
        }
      }, {
        "name" : "yarn-RESOURCEMANAGER-7be275fc706044f09590a812053baca2",
        "type" : "RESOURCEMANAGER",
        "hostRef" : {
          "hostId" : "b24c7526-57ef-4d95-9146-6c38e889e9bb"
        },
        "config" : {
          "items" : [ {
            "name" : "rm_id",
            "value" : "106"
          }, {
            "name" : "role_jceks_password",
            "value" : "7kyotowxxbusz4jm087e0oski"
          } ]
        }
      } ],
      "displayName" : "YARN (MR2 Included)"
    }, {
      "name" : "hive",
      "type" : "HIVE",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "HIVEMETASTORE",
          "items" : [ {
            "name" : "hive_metastore_java_heapsize",
            "value" : "52428800"
          } ]
        }, {
          "roleType" : "HIVESERVER2",
          "items" : [ {
            "name" : "hiveserver2_java_heapsize",
            "value" : "52428800"
          }, {
            "name" : "hiveserver2_spark_driver_memory",
            "value" : "966367641"
          }, {
            "name" : "hiveserver2_spark_executor_cores",
            "value" : "4"
          }, {
            "name" : "hiveserver2_spark_executor_memory",
            "value" : "912680550"
          }, {
            "name" : "hiveserver2_spark_yarn_driver_memory_overhead",
            "value" : "102"
          }, {
            "name" : "hiveserver2_spark_yarn_executor_memory_overhead",
            "value" : "153"
          } ]
        } ],
        "items" : [ {
          "name" : "hive_metastore_database_host",
          "value" : "ec2-35-167-64-53.us-west-2.compute.amazonaws.com"
        }, {
          "name" : "hive_metastore_database_name",
          "value" : "hive"
        }, {
          "name" : "hive_metastore_database_password",
          "value" : "hive"
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hive-GATEWAY-49730cc9b75563a071086a68836a0f68",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "34dc2f98-44e4-48bb-9b9c-d2a3283e0a56"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-4c7d33ab85eb65a18f81f29a049724b0",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "2e882be2-3f62-4bd2-a3d1-a4e52ad18ff1"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-62df31e1595c36f8802fabd4c07f0faf",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "31710729-d236-402a-9c76-795406c8d203"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-7be275fc706044f09590a812053baca2",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "b24c7526-57ef-4d95-9146-6c38e889e9bb"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-8953e23ba3c26181b46a7f4e7779f088",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "61e435e3-259c-45ed-b9af-81fa75be7f17"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-HIVEMETASTORE-4c7d33ab85eb65a18f81f29a049724b0",
        "type" : "HIVEMETASTORE",
        "hostRef" : {
          "hostId" : "2e882be2-3f62-4bd2-a3d1-a4e52ad18ff1"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "d2cjri1d8dotvfrk9jgfvymqn"
          } ]
        }
      }, {
        "name" : "hive-HIVESERVER2-49730cc9b75563a071086a68836a0f68",
        "type" : "HIVESERVER2",
        "hostRef" : {
          "hostId" : "34dc2f98-44e4-48bb-9b9c-d2a3283e0a56"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "dm65187djwdv4hgprj4mhnnxu"
          } ]
        }
      } ],
      "displayName" : "Hive"
    }, {
      "name" : "oozie",
      "type" : "OOZIE",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "OOZIE_SERVER",
          "items" : [ {
            "name" : "oozie_database_host",
            "value" : "ec2-35-167-64-53.us-west-2.compute.amazonaws.com"
          }, {
            "name" : "oozie_database_password",
            "value" : "oozie"
          }, {
            "name" : "oozie_database_type",
            "value" : "mysql"
          }, {
            "name" : "oozie_database_user",
            "value" : "oozie"
          }, {
            "name" : "oozie_java_heapsize",
            "value" : "52428800"
          } ]
        } ],
        "items" : [ {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "oozie-OOZIE_SERVER-8953e23ba3c26181b46a7f4e7779f088",
        "type" : "OOZIE_SERVER",
        "hostRef" : {
          "hostId" : "61e435e3-259c-45ed-b9af-81fa75be7f17"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "c2hpzflbp2k8l8ait5hxtqnud"
          } ]
        }
      } ],
      "displayName" : "Oozie"
    }, {
      "name" : "hue",
      "type" : "HUE",
      "config" : {
        "roleTypeConfigs" : [ ],
        "items" : [ {
          "name" : "database_host",
          "value" : "ec2-35-167-64-53.us-west-2.compute.amazonaws.com"
        }, {
          "name" : "database_password",
          "value" : "hue"
        }, {
          "name" : "database_type",
          "value" : "mysql"
        }, {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "hue_service_safety_valve",
          "value" : "[desktop]\nallowed_hosts=*"
        }, {
          "name" : "hue_webhdfs",
          "value" : "hdfs-NAMENODE-62df31e1595c36f8802fabd4c07f0faf"
        }, {
          "name" : "oozie_service",
          "value" : "oozie"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hue-HUE_SERVER-62df31e1595c36f8802fabd4c07f0faf",
        "type" : "HUE_SERVER",
        "hostRef" : {
          "hostId" : "31710729-d236-402a-9c76-795406c8d203"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "5yqsaktfjy0wa3vczgfmnq0iu"
          }, {
            "name" : "secret_key",
            "value" : "kIC1v0qEMtJzaEc6rwamBEiJUn3kC6"
          } ]
        }
      } ],
      "displayName" : "Hue"
    } ]
  } ],
  "hosts" : [ {
    "hostId" : "b24c7526-57ef-4d95-9146-6c38e889e9bb",
    "ipAddress" : "172.31.10.236",
    "hostname" : "ip-172-31-10-236.us-west-2.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "2e882be2-3f62-4bd2-a3d1-a4e52ad18ff1",
    "ipAddress" : "172.31.10.48",
    "hostname" : "ip-172-31-10-48.us-west-2.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "34dc2f98-44e4-48bb-9b9c-d2a3283e0a56",
    "ipAddress" : "172.31.14.125",
    "hostname" : "ip-172-31-14-125.us-west-2.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "31710729-d236-402a-9c76-795406c8d203",
    "ipAddress" : "172.31.2.148",
    "hostname" : "ip-172-31-2-148.us-west-2.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "61e435e3-259c-45ed-b9af-81fa75be7f17",
    "ipAddress" : "172.31.7.46",
    "hostname" : "ip-172-31-7-46.us-west-2.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  } ],
  "users" : [ {
    "name" : "__cloudera_internal_user__mgmt-EVENTSERVER-7be275fc706044f09590a812053baca2",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "e873b10572f0e1e2c8ca0e6ff1dc23149d64cb83ffdc33a4f7c2362737537750",
    "pwSalt" : -7207666544847746053,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-HOSTMONITOR-7be275fc706044f09590a812053baca2",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "b87e59987696e1ba3f53fe7f9fe9565c495b4e9924a922a58976f05597bb0582",
    "pwSalt" : 6794749196345263319,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-REPORTSMANAGER-7be275fc706044f09590a812053baca2",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "c1266c7166e77b8e955f89bd3815ab3f13a3289dca57eff4c7a39763b0946b6a",
    "pwSalt" : -8895614302631683516,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-SERVICEMONITOR-7be275fc706044f09590a812053baca2",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "72f295d5c047febaddb1b6878a55244f74a8444ff1cd1996730f3a63ee443d73",
    "pwSalt" : -3325748172907521663,
    "pwLogin" : true
  }, {
    "name" : "admin",
    "roles" : [ "ROLE_LIMITED" ],
    "pwHash" : "0c544c721deafcbfa5db3dc864a7e941c2f11f566bf1d0a6103b7b2b7b56f178",
    "pwSalt" : 2529111403183372628,
    "pwLogin" : true
  }, {
    "name" : "minotaur",
    "roles" : [ "ROLE_CONFIGURATOR" ],
    "pwHash" : "2a2c97c47cd0eedac6bbf9bf93050e10b82ec47e9729f7f68a5fb8f2f634d715",
    "pwSalt" : 5615409857029462742,
    "pwLogin" : true
  }, {
    "name" : "msmarnaoui",
    "roles" : [ "ROLE_ADMIN" ],
    "pwHash" : "b7faa11a94a50565a0d810c576f61a7d8774ed9e214ef84fdb9ebc8e9203422a",
    "pwSalt" : 4931120607206686820,
    "pwLogin" : true
  } ],
  "versionInfo" : {
    "version" : "5.10.0",
    "buildUser" : "jenkins",
    "buildTimestamp" : "20170120-1037",
    "gitHash" : "aa0b5cd5eceaefe2f971c13ab657020d96bb842a",
    "snapshot" : false
  },
  "managementService" : {
    "name" : "mgmt",
    "type" : "MGMT",
    "config" : {
      "roleTypeConfigs" : [ {
        "roleType" : "EVENTSERVER",
        "items" : [ {
          "name" : "event_server_heapsize",
          "value" : "593494016"
        } ]
      }, {
        "roleType" : "HOSTMONITOR",
        "items" : [ {
          "name" : "firehose_heapsize",
          "value" : "593494016"
        }, {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "805306368"
        } ]
      }, {
        "roleType" : "REPORTSMANAGER",
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
      }, {
        "roleType" : "SERVICEMONITOR",
        "items" : [ {
          "name" : "firehose_heapsize",
          "value" : "593494016"
        }, {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "805306368"
        } ]
      } ],
      "items" : [ ]
    },
    "roles" : [ {
      "name" : "mgmt-ALERTPUBLISHER-7be275fc706044f09590a812053baca2",
      "type" : "ALERTPUBLISHER",
      "hostRef" : {
        "hostId" : "b24c7526-57ef-4d95-9146-6c38e889e9bb"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "6qkye49z3p5ggyi6ljx9su7at"
        } ]
      }
    }, {
      "name" : "mgmt-EVENTSERVER-7be275fc706044f09590a812053baca2",
      "type" : "EVENTSERVER",
      "hostRef" : {
        "hostId" : "b24c7526-57ef-4d95-9146-6c38e889e9bb"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "54xkdxf3bpe9gsfpdlfe5o5gg"
        } ]
      }
    }, {
      "name" : "mgmt-HOSTMONITOR-7be275fc706044f09590a812053baca2",
      "type" : "HOSTMONITOR",
      "hostRef" : {
        "hostId" : "b24c7526-57ef-4d95-9146-6c38e889e9bb"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "9fz2wi0oi4g8jdc2yp5kfx39"
        } ]
      }
    }, {
      "name" : "mgmt-REPORTSMANAGER-7be275fc706044f09590a812053baca2",
      "type" : "REPORTSMANAGER",
      "hostRef" : {
        "hostId" : "b24c7526-57ef-4d95-9146-6c38e889e9bb"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "7fjmhqo488amn1705z2o0nfqf"
        } ]
      }
    }, {
      "name" : "mgmt-SERVICEMONITOR-7be275fc706044f09590a812053baca2",
      "type" : "SERVICEMONITOR",
      "hostRef" : {
        "hostId" : "b24c7526-57ef-4d95-9146-6c38e889e9bb"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "3ikzr4feayrz5idvns6few6z4"
        } ]
      }
    } ],
    "displayName" : "Cloudera Management Service"
  },
  "managerSettings" : {
    "items" : [ {
      "name" : "CLUSTER_STATS_START",
      "value" : "10/22/2012 9:30"
    }, {
      "name" : "PUBLIC_CLOUD_STATUS",
      "value" : "ON_PUBLIC_CLOUD"
    }, {
      "name" : "REMOTE_PARCEL_REPO_URLS",
      "value" : "https://archive.cloudera.com/cdh5/parcels/{latest_supported}/,https://archive.cloudera.com/cdh4/parcels/latest/,https://archive.cloudera.com/impala/parcels/latest/,https://archive.cloudera.com/search/parcels/latest/,https://archive.cloudera.com/accumulo/parcels/1.4/,https://archive.cloudera.com/accumulo-c5/parcels/latest/,https://archive.cloudera.com/kafka/parcels/latest/,https://archive.cloudera.com/navigator-keytrustee5/parcels/latest/,https://archive.cloudera.com/spark/parcels/latest/,https://archive.cloudera.com/sqoop-connectors/parcels/latest/"
    } ]
  }
}
```
