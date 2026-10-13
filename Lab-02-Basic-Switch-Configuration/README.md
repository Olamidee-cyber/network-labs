# Lab 02 — Basic Switch Configuration

## Objective

Configure and manage a Cisco 2960 switch using the Cisco IOS CLI.

## Topology

- 1 Cisco 2960 switch
- 2 PCs
- PC0: 192.168.10.10/24
- PC1: 192.168.10.20/24
- Switch management IP: 192.168.10.2/24

## Configuration

The switch was configured with:

- Hostname: SW1
- Enable secret
- Console password
- VLAN 1 management interface
- Startup configuration

## Commands Practiced

```text
enable
configure terminal
hostname SW1
enable secret class
line console 0
interface vlan 1
ip address 192.168.10.2 255.255.255.0
no shutdown
show ip interface brief
show mac address-table
show vlan brief
copy running-config startup-config
