
# STEP 1

<strong> Operating system required memory </strong>

* The spreadsheet derived value : 7 Go (which is too high): 

* My Value : 2.5 Go 

<strong>Explanation: </strong>
 
As per <strong>the official documentation od RedHat 7 </strong>,  Red Hat Enterprise Linux Atomic Host also requires 1 GB of memory to run after being installed, but installation on bare metal hardware (not as a virtualization host) requires 2 GB of RAM.

URL: https://access.redhat.com/documentation/en-US/Red_Hat_Enterprise_Linux/7/html/Installation_Guide/sect-installation-planning-disk-space-memory-x86.html

<strong> yarn.nodemanager.resource.cpu-vcores </strong>

* The spreadsheet derived value : 4               

* My Value : 6               

<strong>Explanation: </strong>
 this parameter shows the  Number of virtual CPU cores that can be allocated for containers. ih its value is reached,  other jobs do not launch until the running jobs finish returning resources back to the node manager. note that I have 8 Vcores per machine
 

# STEP 2

Workload factor will help cluster to better manage the different workload : interactive , Batch workload or mixed.
 
