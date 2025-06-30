---
created: 2025-06-27T15:26:00
---
---

## 🔤 IPV4 Classes 
---
> IPV4 consists of *==5 Classes*==

* ### Classes
	* A : `1 - 127`
	* B : `128 - 191`
	* C : `192 - 223`
	* D : `224 - 239`  *Multicasting*
	* E : `240 - 254`  *Research + GOV*
		here class : `A , B , C` are used for ==Host== (*laptop , printer , router , switch , firewall , lan , camera*)


## 🥅 Classes & Their Subnet Mask
---
> here we will see which class consist of their subnet , easier to detect the range 

* ### Class (A - C)
	* A : `255.0.0.0`
	* B : `255.255.0.0`
	* C : `255.255.255.0`

		- another thing is we can't assign a class `D , E` addressed , configuring to them will result in Invalid IP address

---


## ❓Why 255 ? 
---
> why 255 and why not 300 ? or any other number in subnet ? 

* ### Reason 
	* `128 + 64 + 32 + 16 + 8 + 4 + 2 + 1`
	* `1     1    1    1    1   1   1   1`
	* if we add *all 1 here* and proceed to ==*sum*== it
	* total = *==255==*


## 🥅 What is Subnet Mask ? 
---
* ### Precisely
	* it tells me what ==*network*== im actually on .
	* consisting of somthing called as *network portion* and a *host portion*


## 🕸️CIDR 
---
> you can spot the CIDR on the side of subnet mask *eg - /24*


* ### How is it formed ?
	> its formed with a subnet mask and some logic of binary (on and off)

```
255.255.255.0
1111111111.11111111.11111111.00000000
8         +     8   +   8 = 24 
```

* in the above eg as we learned `255` = 1 and `0` = 0 , 
* as each octet is of `8 Bits`
* to get the CIDR from an Subnet mask 
* add the 8 bits of `1` where 255 consist's making it a CIDR 24 for a class C address
> hence the complete result is 192.168.100.1 / 255.255.255.0 / 24


* ### Every Class CIDR
	* A : `/8`
	* B : `/16`
	* C : `/24`



## 😲 True range of CLASS A and Pinging the NIC 
---
> here we will understand what is NIC and the loopback Address

* ### Class A*
	* the class A range comes within `1 - 127` as we learned.
	* however , the true range is `1 - 126`
	* why ? , the *`127`* is loopback address , or also identifying  ==NIC== 

* ### LoopBack Address
	* Testing network software and TCP/IP stack itself
	* allows application to *communicate* with ==themselves== on *==same machine==*
	* verifies that ==*network*== stack is working correctly
	* *eg* `127.0.0.1` is a *loopback address*

* ### NIC
	* *Network Interface card* a piece of ==hardware== allows us to connect to a *network*
	* acts a ==*intermediary*== , enabling device to send and recieve data over a network
	* can be wired using ==ethernet== and also using ==WI-FI==

* ### Verifying the working of NIC Card*
	* if we ==ping== `127.0.0.1`
	* and the ==ICMP== packets happen to respond correctly that means 
	  my *==NIC==* is working properly
	* if add `127.0.0.1` as a IP config it will give ==invalid Ip== error

