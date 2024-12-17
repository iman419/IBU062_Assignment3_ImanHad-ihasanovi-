PC0 PC-PT 169.254.91.214/16
PC1 PC-PT 169.254.102.202/16
Laptop0 Laptop-PT 169.254.104.147/16
Server0 Server-PT 169.254.100.137/16
Switch0 2960 IOS15 Switch
Router0 1941 Router 
Switch1 2960 IOS15 Switch
Server1 Server-PT 169.254.69.89/16
Server2 Server-PT 169.254.109.125/16

Router(config)#ip DHCP excluded-address 168.90.0.1 168.90.0.9
Router(config)#ip DHCP pool POOL-1
Router(dhcp-config)#network 168.90.0.0 255.255.0.0
Router(dhcp-config)#default-router 168.90.0.1
Router(config)#ip DHCP excluded-address 210.3.14.1 210.3.14.9
Router(config)#ip DHCP pool POOL-2
Router(dhcp-config)#network 210.3.14.0 255.255.255.0
Router(dhcp-config)#default-router 210.3.14.1
