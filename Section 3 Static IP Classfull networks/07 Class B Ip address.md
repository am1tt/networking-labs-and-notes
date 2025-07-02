---
created: 2025-07-02T12:12:00
---
---

## 🅱️ Class B
---
> here we will look the Class B address overview 

* ### Range
	* Class B range : `128 - 191`

* ### Network & Host portion
	* consist of 2 `network portion`
	* consist of 2 `Host portion`


* ### Class B Address & Subnet Mask
	* Address : `172.16.100.1`
	* Subnet Mask : `255.255.0.0`

* ### NID and Broadcast ( Class B )
	* NID : `172.16.0.0`
	* Broadcast : 172.16.255.255

* ### First and last host
	* First host : `172.16.0.1`
	* Last host : `172.16.255.254`

* ### Subnet and CIDR ( Class B )
	* as subnet is : `255.255.0.0`
	* meaning `16` bits for *network portion* and `16` bits for *Host*
	* resulting the CIDR of `/16` for *Class B*

* ### Network portion
	* looking at the previous class c , in class b 
	* network portion matters but is different that class c
	* eg : `172.16.100.200` can communicate with `172.16.140.4`
	* why ? because `172` aand `16` is the network portion and the other are host



## 🤔Some different things 
---
* ### Working of 255 in class B
	[255 address](screenshots/class-b/proof-255-ip.png)
	* in the above image you can see
	* in class b adress we can include `255` on both host portion 
	* if the numbers are are different 
	* eg : `172.16.255.0` or `172.16.0.255` or any number other than 0
	* and also `172.16.254.255` or `172.16.255.254`

* ### Another example 
	* [last address ICMP](screenshots/class-b/last-address-ping.png)
		* in the above screenshot , we pinged the last ip host of class B 
		* `172.16.254.255`


## 🔢 Number of Hosts ( Class B )
---
> to count the host , it consist of base value and its bits of host and subtracting the NID and Broadcast

* Take the base of `2`
* Bits of the host here the Bits of host is : `16`
* take `2` NID and Broadcast for `subraction`
```
 2 (base) ^ 16 (host) - 2 (Nid & Bd) = 65532 Hosts 
```


