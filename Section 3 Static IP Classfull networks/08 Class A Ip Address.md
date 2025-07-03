---
created: 2025-07-03T14:15:00
---
---


## ➡️ Class A summary
---
> we cannot count 127 here as it counts in loopback address

* Class A range is : `1 - 126`
* Loopback : `127` for *ICMP* the NIC
* Network portion : `1` (*8 bits*)
* Host portion : `3` (*24 bits*)

* ### Example of Class A Address
	* address : `10.0.2 1`
	* subnet mask : `255.0.0.0`
	* CIDR Range : `8`

* ### NID & Broadcast
	* NID : `10.0.0.0`
	* Broadcast : `10.255.255.255`

* ### First & Last Host
	* First Host : `10.0.0.1`
	* Last host : `10.255.255.254`
	
* ### Calculation Hosts In class A
	* `2(base) - 24(bits,host) - 2(bd , NID) = 16777214`
	* this states class A contains a maximum amount of host than any *class*
