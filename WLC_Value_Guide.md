[back](./README.md)
# WLC
## General Settings
### CAPWAP Wirelsss
#### Security
##### Server (specific radius server)
###### Address
    IP Address
###### Port
    Port Number (ie 1812)
###### Secret
    Password for Radius Server
    
#### Wireless LANs
    List of named WLANS
#### WLAN Name (ie GUEST WIFI, Office WIFI)
##### Enabled
Value | Setting
------------ | -------------
0 | Disabled
1 | Enabled
##### Security Mode
###### Authen Type
Value | Setting
------------ | -------------
0 | none
1 | WEP
2 | PSK (WPA)
3 | 802.1x (WPA)
4 | PSK (WPA2)
5 | 802.1X (WPA2)
###### Encryption Type
Value | Setting
------------ | -------------
0 | none
1 | WEP 40 bit key
2 | WEP 104 bit key
3 | TKIP
4 | AES
###### Pass Phrase
    WPA Pass Phrase
###### Radius Server Address
    Radius Server IP Address
###### Radius Shared Secret
    Radius Server Shared Secret
###### WEP Key
    WEP Key
##### SSID
    WLAN Name
##### VLAN
    VLAN #
  
---

### DHCP Server List
### DHCP Server
#### DHCP Enable
#### Pools
##### Pool Name
###### Default Gateway
    Default Gateway
###### DNS Server
    DNS Server
###### Domain Name
    Domain Name
###### Max User
    Maximum number of DHCP clients
###### Name
    Name of Pool
###### Network Address
    Network Address of Pool
###### Start IP address
    Starting IP Address
###### Subnet Mask
    Subnet Mask
###### TFTP Server
    TFTP Server
###### WLC Address
    WLC Address






---

### Port
#### PortType (ie GigabitEthernet 0/0/0, Guest WIFI, Office WIFI)


##### DHCP Server IP
    IP of DHCP Server

##### IP Address
    IP Address of Interface

##### Physcial Port Number
    Physical Port Number of Interface
  
##### Port Gateway
    Default Gateway of Interface
  
##### Port Status
Value | Setting
------------ | -------------
0 | Disabled
1 | Enabled
  
##### Subnet Mask
    Subnet Mask
  
##### VLAN Identifier
    VLAN #
  
---

### SNMP
#### TRAP Receivers
##### Trap Reciever 1 (Specific Trap Reciever)
###### Community Name
    SNMP Community Name
###### Enabled
Value | Setting
------------ | -------------
0 | Disabled
1 | Enabled
###### Receiver IP
    IP of Reciever
