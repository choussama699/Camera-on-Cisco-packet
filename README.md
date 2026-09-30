# Camera-on-Cisco-packet

A simple IoT lab in Cisco Packet Tracer where two IP cameras and a PC are connected to a Cisco 2960 switch in a single 192.168.1.0/24 network. It shows how IoT devices join a LAN and how a PC can reach them.


Topology
Device	  Type	    IP Address	Subnet Mask  	Connected To
PC0	      PC	      192.168.1.1	255.255.255.0	Switch0
Camera 1  IP Camera	192.168.1.2	255.255.255.0	Switch0
Camera 2	IP Camera	192.168.1.3	255.255.255.0	Switch0

All devices are in the same subnet and VLAN, so no router or default gateway is needed.


Verification : 

From PC0 :
ping 192.168.1.2
ping 192.168.1.3

Successful replies confirm that both cameras are reachable. On the switch

show mac address-table
show ip interface brief
