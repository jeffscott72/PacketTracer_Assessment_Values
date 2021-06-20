[back](./README.md)
# Switch Settings
---
## General Settings
### Banner MOTD
    Provide a literal value for the MOTD message, can use Regular Expressions to search for patterns (see examples below)
#### Match anything, has to be at least one character
    {{RegEx:.+}} 
#### Matches the KEYWORD and anything character(s) before or after it.
    {{RegEx:.*KEYWORD.*}}
### CDP
Value | Setting
------------ | -------------
0	| Disabled
1	| Enabled

### LLDP
Value | Setting
------------ | -------------
0	| Disabled
1	| Enabled

---
## DHCP Snooping
### Enabled
Value | Setting
------------ | -------------
0 | Disabled
1 | Enabled
 

### Mac Address Verified
Value | Setting
------------ | -------------
0 | Disabled
1 | Enabled

### Option 82 Inserted ???
Value | Setting
------------ | -------------
0 | Disabled
1 | Enabled

### Option 82 Trusted
Value | Setting
------------ | -------------
0 | Do Not Allow Untrusted
1 | Allow Untrusted


### VLANS
    List of VLANS

---

## DNS

### IP Domain-Lookup
Value | Setting
------------ | -------------
0 | Disabled
1 | Enabled

---

## DAI
### VLANS
    List of VLANS

### Validate:
#### Dst-mac
Value | Setting
------------ | -------------
0 | Disabled
1 | Enabled


#### Ip
Value | Setting
------------ | -------------
0 | Disabled
1 | Enabled

#### Src-mac
Value | Setting
------------ | -------------
0 | Disabled
1 | Enabled

---

## SwitchPort Settings:

### Bpduguard
Value | Setting
------------ | -------------
0 | Disabled
1 | Enabled

### CDP Enabled
Value | Setting
------------ | -------------
0 | Disabled
1 | Enabled

### DCHP Snooping Trust
Value | Setting
------------ | -------------
0 | Not Trusted
1 | Trusted

### Dynamic Mode
Value | Setting
------------ | -------------
0 | Dynamic Desirable
1 | Dynamic Auto
2 | Trunk
3 | Access

### LLDP Receive
Value | Setting
------------ | -------------
0 | Disabled
1 | Enabled

### LLDP Transmit
Value | Setting
------------ | -------------
0 | Disabled
1 | Enabled

### Nonegotiate
Value | Setting
------------ | -------------
0	| False
1	| True

### Port Mode
Value | Setting
------------ | -------------
0 	| Trunk
1 	| Access

### Port Status
Value | Setting
------------ | -------------
0	| Down
1	| Up

### Port Type
Value | Setting
------------ | -------------
2	| Ethernet (NM-1CE)
3	| FastEthernet
4	| GigabitEthernet
5	| FastEthernet Fiber
6	| GigabitEthernet Fiber
8	| Serial (NIM2T)
12	| Wireless (NIM-1W 2.4GHz)
13	| Wireless (WMP300N)
18	| Modem (NM-1AM)
24	| Wireless (NIM-1WA 5GHz)
37	| Wireless (NIM-FG/4G
46	| Wireless (NIM-1WAC 2.4/5GHz)


### Port Up
Value | Setting
------------ | -------------
0	| False
1	| True

### PortFast
Value | Setting
------------ | -------------
0 | ??? 
1 | ???

### Root Guard
Value | Setting
------------ | -------------
0 | ???
1 | ???

### SwitchPort Protected
Value | Setting
------------ | -------------
0 | ???
1 | ???

---

## VLAN Port Settings:
### Description
    Provide a literal value for the interface description,  
    can use Regular Expressions to search for patterns (see examples below)
#### Match anything, has to be at least one character
    {{RegEx:.+}} 
#### Matches the KEYWORD and anything character(s) before or after it.
    {{RegEx:.*KEYWORD.*}}
### IP Address
    IPv4 address of Interface
### Port Status
Value | Setting
------------ | -------------
0	| Down
1	| Up
### Port Up
Value | Setting
------------ | -------------
0	| Down
1	| Up
### Subnet mask
    Subnet Mask of Interface

---

## Security
### Modulus Bits
Value | Setting
------------ | -------------
Number of Bits | 1024, 2048

---

## SSH Server
### Version
Value | Setting
------------ | -------------
0	| Default
1	| Version 1
2	| Version 2

---

## STP

### BPDU Guard Default
Value | Setting
------------ | -------------
0	| Disabled
1 	| Enabled

### PortFast Default
Value | Setting
------------ | -------------
0	| Disabled
1 	| Enabled

### RSTP
Value | Setting
------------ | -------------
0	| PVST
1	| RPVST

### VLANs
Value | Setting
------------ | -------------
VLAN #
Priority
32768

### VLAN Number
VLAN #

---

## VTP

### VTP Mode:
Value | Setting
------------ | -------------
0	| server
1	| client
2	| transparent

---

## VTY Lines

### AAA Method List Name
    Value of: Login Authentication AUTH_LIST

### Logging Sync
Value | Setting
------------ | -------------
0	| Disabled
1	| Enabled

### Login
Value | Setting
------------ | -------------
0	| No Login
1	| Login or Login Authentication AUTH_LIST
2	| Login Local

### Transport Input
Value | Setting
------------ | -------------
0	| None
1	| Telnet
2	| SSH
2147483647	| All

---




