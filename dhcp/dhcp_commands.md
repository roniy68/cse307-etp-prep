en 

config t 

hostname R1

int gig0/0/0

ip add 192.168.1.1 255.255.255.0

no sh


==========
sh ip int br // shows 

====
wr //writes the configuration



*************
DHCP 
**********
ip dhcp pool <name>

default-router 192.168.1.1

network 192.168.1.0 255.255.255.0

<ctr-z>

wr