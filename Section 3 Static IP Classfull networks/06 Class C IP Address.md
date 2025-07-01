---
created: 2025-07-01T12:28:00
---
----

## ©️Class C Address
----
> we know class C falls in range of `192-223`

* IP Address ( C ) : `192.168.100.1`
* Subnet Mask : `255.255.255.0`

* ### Network and Host Portion (*Class C*)
	* `192.168.100.1`
	* `255.255.255.0`
	* in the above mentioned IP and SM , Class C address consist of 3 *network portion* and 1 *Host portion*
	* `how to know that ? , submask consist of 3 (255) or --> 1`
	* `255.255.255.0` making it 3 *network portion* and 1 *host portion*


## 🤔Valid and Invalid ranges 
---

* ### Valid Range 
	* the valid range will be from `192.168.100.1 - 192.168.100.255`
	* *host* portion matters alot when coming to the ranges 
	* as mentioned earlier the differ of *host* portion is done by `subnet mask`

---

[invalid ip range start](screenshots/class-c/invalid-ip-start.png)

* ### Invalid Start Range
	* here in the above image you can see
	* that inserting `192.168.100.0` will result in *invalid ip*
	* because in the host section `0` is considered invalid range and it should start from `1`
---

[invalid IP Ending Range](screenshots/class-c/invalid-ip-end.png)

* ### Invalid End Range
	* in the above image 
	* inserting `192.168.100.255` will result in *invalid ip*
	* because `255` in host portion is considered as the *invalid* and also a *ending* range , as class 3 consist of only `1 host` portion , inserting *255* will result in invalid ip address


* ### Why Invalid start/end host doesn't work ? (`NID and Broadcast`)
	* `192.168.100.0` -> 0 as *host* portion belongs `NID` network ID , this tells what network does it belong to  ,eg we are in class c `192.168.100` network
	* `192.168.100.255` -> 255 as *host* portion is a `Broadcast` means if im sending something it goes to *everyone*
	* can you go over `255` no . why ? refer [[03 IPV4 Classes]] as mentioned the total is `255` as last range



## Class C Network Setup
---
* ### Setup
	* [Setup overiew](screenshots/class-c/class-c-setup.png)
		* in the above image , it is a complete class C Setup (*Statically*)
		* IP ranging from `192.168.100.1 --> 4`
		* meaning it has `4 Hosts` , connected to a intermediary *Switch* 

* ### ICMP the Configured Ip Address
	* [ICMP Screenshot](screenshots/class-c/class-c-same-network.png)
		* here the network `host` configured 
		* testing out `ICMP` (*ping*) and getting a response
		* means they belong to the *`same network`*
		* you can also check your ipaddress & subnet mask with `ipconfig` and `ipconfig /all`


## 🧾Proof of network portion in IP Addresses
---
> the address `192.168.100.1` consist of 3 network portion and 1 *host* portion but how do we proove that ? 

* ### ICMP PDU (Pinging) Different network address
* [PDU Testing Result](screenshots/class-c/pdu-testing.png)
	* in the above image , we changed last two `hosts` to `192.168.200.3` and kept 1 host with `192.168.100.1` and similar one with `2`
	
	* we can see that *network portion* consisting of `100` are able to communicate with each other
	
	* however , `192.168.100.1` can't communicate or response ICMP with `192.168.200.3
	
	* `why ? because they are on different network thus proving the network portion`
	
	* this is where a *router* also comes for working
