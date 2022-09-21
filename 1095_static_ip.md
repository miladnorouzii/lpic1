########## Ubuntu

######### vim /etc/netplan/file
```bash
network:
  version: 2
  renderer: networkd
  ethernets:
    ens3:
      dhcp4: no
      addresses:
        - 192.168.121.221/24
      gateway4: 192.168.121.1
      nameservers:
          addresses: [8.8.8.8, 1.1.1.1]
```	  

netplan try
netplan apply

####### Debian
vim /etc/network/interfaces

```bash
# The loopback network interface
auto lo
iface lo inet loopback
 
# The primary network interface
auto ens36
iface ens36  inet static
 address 192.168.2.236
 netmask 255.255.255.0
 gateway 192.168.2.254
 dns-nameservers 192.168.2.254
```
sudo systemctl restart networking.service

####### centos

cd /etc/sysconfig/network-scripts/
vim ifcfg-ens36

```bash
# static IP address on CentOS 7 or RHEL 7#
TYPE=Ethernet
BOOTPROTO=none
IPADDR=192.168.2.203
PREFIX=24
GATEWAY=192.168.2.254
DNS1=192.168.2.254
DNS2=8.8.8.8
DNS3=8.8.4.4
DEFROUTE=yes
IPV4_FAILURE_FATAL=no
IPV6INIT=no
NAME=eth0
DEVICE=eth0
ONBOOT=yes
```
######## systemctl restart network



 
