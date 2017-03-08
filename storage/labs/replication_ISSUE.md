# Problem: BDR Job fails with unknown host exception

The Backup Host does not recognize the internal IP of the source cluster node to which it connects

# Solution:

Add all the IP, Internal IPs and Private DNS of teh source cluster nodes to the /etc/hosts files of the nodes of the backup cluster.

It works!
