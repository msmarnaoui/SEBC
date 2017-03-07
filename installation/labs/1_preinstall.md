# disable swappines

sudo sysctl vm.swappiness=1

# nscd and ntpd

sudo systemctl start nscd.service

sudo systemctl start ntpd.service

systemctl enable ntpd.service

systemctl enable  nscd.service


# Disable Transparent Huge Pages 

echo never > /sys/kernel/mm/redhat_transparent_hugepage/defrag

