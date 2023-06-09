# Cisco Packet Tracer


# Basic Commands: 


=================================
Basic Router Commands
=================================
Router>                          ---User EXEC mode               exit
Router> ?
Router> enable     
---------------
Router#                          ---Privileged EXEC mode         disable, exit
Router# ?
-----------------
Router# configure terminal
Router(config)#                  ---Global Config mode           exit, end, Ctrl+c, Ctrl+z
Router(config)# ?
-----------------
Router(config)# line vty 0 15
Router(config)# line console 0
Router(config-line)#             ---Line configuration mode      exit, end, Ctrl+c, Ctrl+z
Router(config-line)# ?
----------------------------
Router(config)# interface gigabitEthernet 0/0/0
Router(config-if)#               ---Interface configuration mode exit, end, Ctrl+c, Ctrl+z
Router(config-if)# ?
----------------------------
Router#
Router# configure terminal
Router# show ?
Router# show running-config
Router# copy running-config startup-config
Router# ping 192.168.1.100
Router# traceroute 192.168.1.100
Router# ssh 192.168.1.100 
Router# telnet 192.168.1.100
Router# debug ?
Router# clock set 07:14:00 October 15 2019
Router# reload
---------------------------------
Router(conf)#
Router(conf)# hostname R1
Router(conf)# banner motd "No unauthorized access allowed!"
Router(conf)# enable password class
Router(conf)# enable secret class
Router(conf)# service password-encryption
Router(config)# line vty 0 15
Router(config)# line console 0
Router(config)# interface gigabitEthernet 0/0/0
----------------------------------------------------
Router(config-line)# 
Router(config-line)# password cisco
Router(config-line)# login
Router(config-line)# transport input all   (line vty)
----------------------------------------------------
Router(config-if)# 
Router(config-if)# interface gigabitEthernet 0/0/0
Router(config-if)# int g0/0                              //command abbreviation
Router(config-if)# ip address 192.168.1.1 255.255.255.0 
Router(config-if)# no shutdown


=================================
Basic Switch Commands
=================================
Switch>                          ---User EXEC mode               exit
Switch> enable     
---------------
Switch#                          ---Privileged EXEC mode         disable, exit
-----------------
Switch# configure terminal
Switch(config)#                  ---Global Config mode           exit, end, Ctrl+c, Ctrl+z
-----------------
Switch(config)# line vty 0 15
Switch(config)# line console 0
Switch(config-line)#             ---Line configuration mode      exit, end, Ctrl+c, Ctrl+z
----------------------------
Switch(config)# interface vlan 1
Switch(config-if)#               ---Interface configuration mode exit, end, Ctrl+c, Ctrl+z
----------------------------
Switch#
Switch# configure terminal
Switch# show ?                
Switch# show running-config
Switch# copy running-config startup-config
Switch# ping 192.168.1.100
Switch# traceroute 192.168.1.100
Switch# ssh 192.168.1.100 
Switch# telnet 192.168.1.100
Switch# debug ?
Switch# clock set 07:14:00 October 15 2019
Switch# reload
---------------------------------
Switch(conf)#
Switch(conf)# hostname R1
Switch(conf)# banner motd "No unauthorized access allowed!"
Switch(conf)# enable password class
Switch(conf)# enable secret class
Switch(conf)# service password-encryption
Switch(config)# line vty 0 15
Switch(config)# line console 0
Switch(config)# interface vlan 1
----------------------------------------------------
Switch(config-line)# 
Switch(config-line)# password cisco
Switch(config-line)# login
Switch(config-line)# transport input all   (line vty)
----------------------------------------------------
Switch(config-if)# 
Switch(config-if)# interface vlan 1
Switch(config-if)# ip address 192.168.1.2 255.255.255.0 
Switch(config-if)# no shutdown
Switch(config-if)# exit
Switch(config)# ip default-gateway 192.168.1.1


Extra helpful commands:
=========================
Router(conf)# no ip domain-lookup       //prevents miss-typed commands from being "translated..." 
Router(conf-line)# logging synchronous  //prevents logging output from interrupting your command input



basic-router-switch-commands.txt
Displaying basic-router-switch-commands.txt.

