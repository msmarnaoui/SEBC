>**cloud provider** *AWS*

>**Nodes IPs and Names**

	35.156.15.161 	ip-172-31-25-25.eu-central-1.compute.internal
	35.156.110.156	ip-172-31-21-243.eu-central-1.compute.internal
	35.157.242.34	ip-172-31-17-144.eu-central-1.compute.internal
	35.157.247.247	ip-172-31-23-122.eu-central-1.compute.internal
	35.158.4.243	ip-172-31-23-237.eu-central-1.compute.internal


>**Linux release** *Red Hat Enterprise Linux Server release 7.3*

>**Disk Capacity FOR EACH NODE**
>
	[root@ip-172-31-25-25 ~]# df -h
	Filesystem      Size  Used Avail Use% Mounted on
	/dev/xvda2       70G  1.5G   69G   3% /
	devtmpfs        7.3G     0  7.3G   0% /dev
	tmpfs           7.2G     0  7.2G   0% /dev/shm
	tmpfs           7.2G   17M  7.2G   1% /run
	tmpfs           7.2G     0  7.2G   0% /sys/fs/cgroup
	tmpfs           1.5G     0  1.5G   0% /run/user/1000
	tmpfs           1.5G     0  1.5G   0% /run/user/0


	[root@ip-172-31-23-237 ~]# df -h
	Filesystem      Size  Used Avail Use% Mounted on
	/dev/xvda2       70G  1.5G   69G   3% /
	devtmpfs        7.3G     0  7.3G   0% /dev
	tmpfs           7.2G     0  7.2G   0% /dev/shm
	tmpfs           7.2G   17M  7.2G   1% /run
	tmpfs           7.2G     0  7.2G   0% /sys/fs/cgroup
	tmpfs           1.5G     0  1.5G   0% /run/user/1000
	tmpfs           1.5G     0  1.5G   0% /run/user/0


	[root@ip-172-31-21-243 ~]# df -h
	Filesystem      Size  Used Avail Use% Mounted on
	/dev/xvda2       70G  1.5G   69G   3% /
	devtmpfs        7.3G     0  7.3G   0% /dev
	tmpfs           7.2G     0  7.2G   0% /dev/shm
	tmpfs           7.2G   17M  7.2G   1% /run
	tmpfs           7.2G     0  7.2G   0% /sys/fs/cgroup
	tmpfs           1.5G     0  1.5G   0% /run/user/1000
	tmpfs           1.5G     0  1.5G   0% /run/user/0


	[root@ip-172-31-17-144 ~]# df -h
	Filesystem      Size  Used Avail Use% Mounted on
	/dev/xvda2       70G  1.5G   69G   3% /
	devtmpfs        7.3G     0  7.3G   0% /dev
	tmpfs           7.2G     0  7.2G   0% /dev/shm
	tmpfs           7.2G   17M  7.2G   1% /run
	tmpfs           7.2G     0  7.2G   0% /sys/fs/cgroup
	tmpfs           1.5G     0  1.5G   0% /run/user/1000
	tmpfs           1.5G     0  1.5G   0% /run/user/0

	[root@ip-172-31-23-122 ~]# df -h
	Filesystem      Size  Used Avail Use% Mounted on
	/dev/xvda2       70G  1.5G   69G   3% /
	devtmpfs        7.3G     0  7.3G   0% /dev
	tmpfs           7.2G     0  7.2G   0% /dev/shm
	tmpfs           7.2G   17M  7.2G   1% /run
	tmpfs           7.2G     0  7.2G   0% /sys/fs/cgroup
	tmpfs           1.5G     0  1.5G   0% /run/user/1000
	tmpfs           1.5G     0  1.5G   0% /run/user/0



>**yum repolist enabled command**

	[root@ip-172-31-25-25 ~]# yum repolist enabled
	Loaded plugins: amazon-id, rhui-lb, search-disabled-repos
	repo id                                                     repo name                                                                   status
	rhui-REGION-client-config-server-7/x86_64                   Red Hat Update Infrastructure 2.0 Client Configuration Server 7                  4
	rhui-REGION-rhel-server-releases/7Server/x86_64             Red Hat Enterprise Linux Server 7 (RPMs)                                    14,038
	rhui-REGION-rhel-server-rh-common/7Server/x86_64            Red Hat Enterprise Linux Server 7 RH Common (RPMs)                             209
	repolist: 14,251
	
	[root@ip-172-31-21-243 ~]# yum repolist enabled
	Loaded plugins: amazon-id, rhui-lb, search-disabled-repos
	repo id                                                     repo name                                                                   status
	rhui-REGION-client-config-server-7/x86_64                   Red Hat Update Infrastructure 2.0 Client Configuration Server 7                  4
	rhui-REGION-rhel-server-releases/7Server/x86_64             Red Hat Enterprise Linux Server 7 (RPMs)                                    14,038
	rhui-REGION-rhel-server-rh-common/7Server/x86_64            Red Hat Enterprise Linux Server 7 RH Common (RPMs)                             209
	repolist: 14,251


	[root@ip-172-31-17-144 ~]# yum repolist enabled
	Loaded plugins: amazon-id, rhui-lb, search-disabled-repos
	repo id                                                      repo name                                                                  status
	!rhui-REGION-client-config-server-7/x86_64                   Red Hat Update Infrastructure 2.0 Client Configuration Server 7                 4
	!rhui-REGION-rhel-server-releases/7Server/x86_64             Red Hat Enterprise Linux Server 7 (RPMs)                                   14,038
	!rhui-REGION-rhel-server-rh-common/7Server/x86_64            Red Hat Enterprise Linux Server 7 RH Common (RPMs)                            209
	repolist: 14,251

	[root@ip-172-31-23-122 ~]# yum repolist enabled
	Loaded plugins: amazon-id, rhui-lb, search-disabled-repos
	repo id                                                      repo name                                                                  status
	!rhui-REGION-client-config-server-7/x86_64                   Red Hat Update Infrastructure 2.0 Client Configuration Server 7                 4
	!rhui-REGION-rhel-server-releases/7Server/x86_64             Red Hat Enterprise Linux Server 7 (RPMs)                                   14,038
	!rhui-REGION-rhel-server-rh-common/7Server/x86_64            Red Hat Enterprise Linux Server 7 RH Common (RPMs)                            209
	repolist: 14,251

	[root@ip-172-31-23-237 ~]# yum repolist enabled
	Loaded plugins: amazon-id, rhui-lb, search-disabled-repos
	repo id                                                      repo name                                                                  status
	!rhui-REGION-client-config-server-7/x86_64                   Red Hat Update Infrastructure 2.0 Client Configuration Server 7                 4
	!rhui-REGION-rhel-server-releases/7Server/x86_64             Red Hat Enterprise Linux Server 7 (RPMs)                                   14,038
	!rhui-REGION-rhel-server-rh-common/7Server/x86_64            Red Hat Enterprise Linux Server 7 RH Common (RPMs)                            209
	repolist: 14,251

>**/etc/passwd**	

	[root@ip-172-31-25-25 ~]# tail -2 /etc/passwd
	ronaldo:x:2016:1003::/home/ronaldo:/bin/bash
	neymar:x:2010:1004::/home/neymar:/bin/bash
	
>**/etc/group**	
>
	[root@ip-172-31-25-25 ~]# tail -2 /etc/group
	barca:x:1003:
	merengues:x:1004:
