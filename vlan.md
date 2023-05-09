en

config t 

hostname sw1

vlan 10
name sales

vlan 20
name marketing


int f0/3
switchport access vlan 10
switchport mode access

int f0/4
switchport access vlan 20
switchport mode access

show vlan bri

=========

now router:
----
en 
config t 

hostname R1
int f0/0 
ip add 192.168.10.1 255.255.255.0

int f0/1
ip add 192.168.20.1 255.255.255.0

no sh

===

trunk: 
===
int f0/1
switchport access vlan 10
switchport mode access

int f0/2
switchport access vlan 20
swichport mode access