[back](./README.md)
# Switch Settings
---
## General Settings
### Banner MOTD
    Provide a literal value for the MOTD message,  
    can use Regular Expressions to search for patterns (see examples below)
#### Match anything, has to be at least one character
    {{RegEx:.+}} 
#### Matches the KEYWORD and anything character(s) before or after it.
    {{RegEx:.*KEYWORD.*}}

---

### CDP
Value | Setting
------------ | -------------
0	| Disabled
1	| Enabled

---

### Console Line

#### Access Control In
    Incoming IPv4 ACL. Can be number or named ACL.

#### IPv6 Access-Control In
    Incoming IPv6 ACL. Uses Named ACLs

#### Logging Sync
Value | Setting
------------ | -------------
0 | Disabled
1 | Enabled

#### Login
Value | Setting
------------ | -------------
0	| No Login
1	| Login or Login Authentication AUTH_LIST
2	| Login Local


#### MOTD BANNER
    Provide a literal value for the MOTD message,  
    can use Regular Expressions to search for patterns (see examples below)

##### Match anything, has to be at least one character
    {{RegEx:.+}} 

##### Matches the KEYWORD and anything character(s) before or after it.
    {{RegEx:.*KEYWORD.*}}
    
#### Password
    Console password
    
#### Terminal Line Timed out: 
    This is the Exec-Timeout value in milliseconds (1 minute = 60000)    
---

### Default Gateway
    Default gateway IP for the switch
    
---

### DHCP Snooping
#### Enabled
Value | Setting
------------ | -------------
0 | Disabled
1 | Enabled
 

#### Mac Address Verified
Value | Setting
------------ | -------------
0 | Disabled
1 | Enabled

#### Option 82 Inserted ???
Value | Setting
------------ | -------------
0 | Disabled
1 | Enabled

#### Option 82 Trusted
Value | Setting
------------ | -------------
0 | Do Not Allow Untrusted
1 | Allow Untrusted

#### VLANS
    List of VLANS associated with DHCP Snooping

---

### DNS

#### IP Domain Name
    Domain name of the network

#### IP Domain-Lookup
Value | Setting
------------ | -------------
0 | Disabled
1 | Enabled

#### IP Name Server
    IP address of the name server
---

### DAI

#### Validate:
##### Dst-mac
Value | Setting
------------ | -------------
0 | Disabled
1 | Enabled


##### Ip
Value | Setting
------------ | -------------
0 | Disabled
1 | Enabled

##### Src-mac
Value | Setting
------------ | -------------
0 | Disabled
1 | Enabled

#### DAI VLANS
    List of VLANS

---

### Enable Password
    Privileged level password    
---

### Enable Secret
    Privileged level secret
    
---

### Hostname
    Name of the switch
    
----

### IOS Configuration
#### Running Configuration
##### LINES
    Allows you match particular lines of the config
#### Startup Configuration
##### LINES
    Allows you match particular lines of the config
---
### IP Domain Name
    Domain name of the network

---
    
### LLDP
Value | Setting
------------ | -------------
0	| Disabled
1	| Enabled

---

### Ports (Switch Ports)
#### PortName (ie FastEthernet0/1)

##### Access VLAN
    Access VLAN number

##### Bpduguard
Value | Setting
------------ | -------------
0 | Disabled
1 | Enabled

##### CDP Enabled
Value | Setting
------------ | -------------
0 | Disabled
1 | Enabled

##### DCHP Snooping Trust
Value | Setting
------------ | -------------
0 | Not Trusted
1 | Trusted

##### Dynamic Mode
Value | Setting
------------ | -------------
0 | Dynamic Desirable
1 | Dynamic Auto
2 | Trunk
3 | Access

##### LLDP Receive
Value | Setting
------------ | -------------
0 | Disabled
1 | Enabled

##### LLDP Transmit
Value | Setting
------------ | -------------
0 | Disabled
1 | Enabled

##### Native VLAN
    Native VLAN number

##### Nonegotiate
Value | Setting
------------ | -------------
0	| Disabled
1	| Enabled

##### Port Mode
Value | Setting
------------ | -------------
0 	| Trunk
1 	| Access

###### Port Security
###### Aging Time
    Aging time in minutes
###### Enabled
Value | Setting
------------ | -------------
0	| Disabled
1	| Enabled
###### Maximum Static MACs
    Total MACs allowed
###### Port Security Violation
Value | Setting
------------ | -------------
0	| Shutdown
1	| Protect
2   | Restrict
###### Sticky Enabled
Value | Setting
------------ | -------------
0	| Disabled
1	| Enabled

##### Port Status
Value | Setting
------------ | -------------
0	| Down
1	| Up

##### Port Type
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


##### Port Up
Value | Setting
------------ | -------------
0	| Off
1	| On

##### PortFast
Value | Setting
------------ | -------------
0 | Disabled
1 | Enabled

##### Root Guard
Value | Setting
------------ | -------------
0 | Disabled
1 | Enabled

##### SwitchPort Protected
Value | Setting
------------ | -------------
0 | Disabled
1 | Enabled

##### Trunk VLANS
    Lists of VLANS that are allowed on Trunk

##### Voice VLAN
    Voice VLAN number

#### VLAN1 (or other VLAN \# if configured)
##### Description
    Provide a literal value for the interface description,  
    can use Regular Expressions to search for patterns (see examples below)
###### Match anything, has to be at least one character
    {{RegEx:.+}} 
###### Matches the KEYWORD and anything character(s) before or after it.
    {{RegEx:.*KEYWORD.*}}
##### IP Address
    IPv4 address of Interface
##### IPv6 Addresses
###### IPv6 Address 1
###### IP Address
    IPv6 address of Interface
###### Prefix Length
    Prefix Length of Interface
##### Link Local
    Link Local IPv6 address of Interface
##### Port Status
Value | Setting
------------ | -------------
0	| Down
1	| Up
##### Port Up
Value | Setting
------------ | -------------
0	| Down
1	| Up
##### Subnet mask
    Subnet Mask of Interface

---

### Power
Value | Setting
------------ | -------------
0 | Off
1 | On

---

### Security
#### Modulus Bits
Value | Setting
------------ | -------------
Number of Bits | 1024, 2048

---

### Service Password Encryption
  Value | Setting
------------ | -------------
0	| Disabled
1 	| Enabled  

---

### SSH Server
#### Version
Value | Setting
------------ | -------------
0	| Default
1	| Version 1
2	| Version 2

---

### STP

#### BPDU Guard Default
Value | Setting
------------ | -------------
0	| Disabled
1 	| Enabled

#### Port Costs
    TODO

#### PortFast Default
Value | Setting
------------ | -------------
0	| Disabled
1 	| Enabled

#### RSTP
Value | Setting
------------ | -------------
0	| PVST
1	| RPVST

#### VLANs
Value | Setting
------------ | -------------
##### VLAN \#
###### Priority
    Default value is: 32768
###### VLAN Number

---

### User Names
#### User Names
    List of usernames and their passwords
---

### VLANS
#### VLAN \#
#### VLAN Name
    Name of VLAN

---

### VTP
#### Domain Name
    Nam of VTP Domain Name

#### VTP Mode:
Value | Setting
------------ | -------------
0	| server
1	| client
2	| transparent

#### VTP Password
    Password used for VTP Domain
    
#### VTP Verion
Value | Setting
------------ | -------------
1	| VTP Version 1
2	| VTP Version 2

---

### VTY Lines
#### VTY Line \#
##### AAA Method List Name
    Value of: Login Authentication AUTH_LIST

##### Access Control In
    Incoming IPv4 ACL. Can be number or named ACL.

##### IPv6 Access-Control In
    Incoming IPv6 ACL. Uses Named ACLs

##### Logging Synch
Value | Setting
------------ | -------------
0	| Disabled
1	| Enabled

##### Login
Value | Setting
------------ | -------------
0	| No Login
1	| Login or Login Authentication AUTH_LIST
2	| Login Local

##### MOTD BANNER
    Provide a literal value for the MOTD message,  
    can use Regular Expressions to search for patterns (see examples below)

###### Match anything, has to be at least one character
    {{RegEx:.+}} 

###### Matches the KEYWORD and anything character(s) before or after it.
    {{RegEx:.*KEYWORD.*}}
    
##### Password
    Provide console password
    
##### Terminal Line Timed out: 
    This is the Exec-Timeout value in milliseconds (1 minute = 60000) 

##### Transport Input
Value | Setting
------------ | -------------
0	| None
1	| Telnet
2	| SSH
2147483647	| All

---




