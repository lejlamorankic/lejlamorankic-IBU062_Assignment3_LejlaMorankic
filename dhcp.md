Step 1. Exclude IPv4 addresses. 
Step 2. Define a DHCPv4 pool name. 
Step 3. Configure the DHCPv4 pool.

Router(config)# ip dhcp excluded-address 168.90.0.1 168.90.0.9
Router(config)# ip dhcp pool POOL-1
Router(dhcp-config)# network 168.90.0.0 255.255.0.0
Router(dhcp-config)# default-router 168.90.0.1
Router(config)# ip dhcp excluded-address 210.3.14.1 210.3.14.9
Router(config)# ip dhcp pool POOL-2
Router(dhcp-config)# network 210.3.14.0 255.255.255.0
Router(dhcp-config)# default-router 210.3.14.1
