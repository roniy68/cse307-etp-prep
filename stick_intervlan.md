config t
hostname sw1

vlan 10
name sales

vlan 20 
name marketing

int range f0/1-2
switchport access vlan 20
switchport mode access

int f0/5
switchport mode trunk
---------

config t
hostname R1

int f0/0
no sh

int f0/0.10
encapsulation dot1q 10
ip add 192.168.10.1 255.255.255.0

int f0/0.20
encapsulation dot1 20
ip add 192.168.20.1 255.255.255.0
===


