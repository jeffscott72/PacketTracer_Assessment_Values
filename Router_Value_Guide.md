[back](./README.md)
# Router
## General Settings
### ACL \#
	Standard ACL Example:
	permit 172.16.0.0 0.0.255.255
	
	Extended ACL Example:
	permit tcp 192.168.1.0 0.0.0.255 192.168.2.0 0.0.0.255 eq www
### ACL NAME
	Standard Named Example:
	deny host 192.168.1.2
	permit any
	
	Extended Named Example:
	permit tcp 192.168.1.0 0.0.0.255 192.168.2.0 0.0.0.255 eq www
	
	

### Banner MOTD
	Provide a literal value for the MOTD message,  
	can use Regular Expressions to search for patterns (see examples below)

#### Match anything, has to be at least one character
	{{RegEx:.+}} 

#### Matches the KEYWORD and anything character(s) before or after it.
	{{RegEx:.*KEYWORD.*}}

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
### DHCP Server
#### Excluded Addresses
	List of excluded IP Addresses
#### Pools
##### PoolName
	Name of pool
###### Default Gateway
	Default gateway
###### DNS Server IP
	IP of DNS Server
###### Network Address
	Network
###### Subnet Mask
	Subnet Mask

----

### DNS
#### IP Domain Name
	Domain name of the network
	
#### IP Domain Name
    Domain name of the network

#### IP Domain-Lookup
Value | Setting
------------ | -------------
0 | Disabled
1 | Enabled	

---

### Enable Password
    Privileged level password    
---

### Enable Secret
    Privileged level secret
    
---

### Hostname
    Name of the switch
    
---

### Login Options
#### Blocking
##### Attempts
	how many login attempts are allowed
##### Duration
	how long to block future login attempts
##### Enabled
Value | Setting
------------ | -------------
0 | Disabled
1 | Enabled
##### Period
	How long you have to use all attempts
---

### NAT
#### Inside Source List
##### Inside Source List:
	Name of pool | Interface (PAT)
#### Inside Source Static
##### NAT Source Setting 1
	inside ip outside ip
	ie 192.168.20.254 209.165.202.130 
#### Pools
##### Pool Name 1
	This one is misleading, it wanted the IP Range of the Pool
	ie 209.165.202.129-209.165.202.129
---

### OSPF
#### Process ID \#

##### Area
###### Area \#
	Area number
	
##### Area Authentication
###### Area \#
	Area number
	
##### Auto Cost
	Autocost value bandwidth reference

##### Default Information
Value | Setting
------------ | -------------
0 | Disabled
1 | Enabled

##### Networks
###### Route\#
	Route being advertised
	ie 11.0.0.0 0.255.255.255 0

##### Passive Interface
###### Default
Value | Setting
------------ | -------------
0 | Disabled
1 | Enabled

###### Specific Interface(s) (ie Gigabit0/0)
Value | Setting
------------ | -------------
0 | Disabled
1 | Enabled

##### Router ID
	Router ID value


---

### Port
#### PortType (ie GigabitEthernet 0/0/0, G0/0/0.10)


##### 802.1Q
###### Native VLAN
	Native VLAN number
###### VLAN ID
	VLAN number	


##### CDP Enabled
Value | Setting
------------ | -------------
0 | Disabled
1 | Enabled	


##### Description
    Provide a literal value for the interface description,  
    can use Regular Expressions to search for patterns (see examples below)
###### Match anything, has to be at least one character
    {{RegEx:.+}} 
###### Matches the KEYWORD and anything character(s) before or after it.
    {{RegEx:.*KEYWORD.*}}
    
##### DHCP Client Enable
value | description
-- | --
0 | Disabled
1 | Enabled


##### Hot Standby
###### Standby 1
###### Preempt
value | description
-- | --
0 | Disabled
1 | Enabled

###### Priority
	Priority value

###### Virtual IP
	Virtual IP address


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


##### NAT MODE
	TODO
Value | Setting
------------ | -------------
0 | Not set
1 | Inside
2 | Outside

##### OSPF Cost
	Cost value

##### OSPF Dead-Interval
	Dead timer
	
##### OSPF Hello-Interval
	Hello timer

##### OSPF Network Type
Value | Setting
------------ | -------------
1	| Point to Piont
5	| Ethernet

##### OSPF Priority
	Priority number
	
	
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

##### Subnet mask
    Subnet Mask of Interface

---

### Power
Value | Setting
------------ | -------------
0 | Off
1 | On

---

### Routes
#### Static Routes
#### Route\# (List of Routes)
	0.0.0.0-0-209.165.200.1-0-254

---

### RoutesV6
#### IPv6 Unicast Routing
Value | Setting
------------ | -------------
0 | Disabled
1 | Enabled

---

### Security
#### Modulus Bits
Value | Setting
------------ | -------------
Number of Bits | 1024, 2048

---

### Security Password Min-Length
	Minimum length of passwords
---

### Service Password Encryption
  Value | Setting
------------ | -------------
0	| Disabled
1 	| Enabled  

---

### SSH Server
#### SSH Authentication Retries
	Number of login attempts
#### SSH Timeout
	How long session can be idle
#### Version
Value | Setting
------------ | -------------
0	| Default
1	| Version 1
2	| Version 2

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
