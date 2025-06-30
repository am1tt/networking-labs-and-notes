---
created: 2025-06-27T14:48:00
---
---

## 👨‍🔬 IP address re-Summary
---
> a common eg of IPv4 Address is *==192.168.100.1==*

* ### We Learned Previously
	* that the base of IP addresses is *==2==*
	* it contains *==4 Octets==*
	* each Octet is *==8 Bits==*
	> also whenever we talk about bits we are talking about *==Binary!*==

---

## ➕✖️ Math Behind it
---
* ### provisions
	* Base is *==2==*
	* one Byte | Octet : *==8 Bits==*

* ### Math
	lets put number base (2) : *==8 Times*== ( 0 - 7 = 8)
	
		2^0 2^1 2^2 2^3 2^4 2^5 2^6 2^7
		1   2   4    8  16  32  64  128
* ### Calculating IP address form it

	    2^0 2^1 2^2 2^3 2^4 2^5 2^6 2^7
		1   2   4    8  16  32  64  128

```
192 : 128 + 64 : 1 , 1 , 0 , 0 , 0 , 0 , 0 , 0 
168 : 128 + 32 + 8 : 1 , 0 , 1 , 0 , 1 , 0 , 0
100 : 64 + 32 + 4 : 0 , 1 , 1 , 0 , 0 , 1 , 0 , 0 
1 : 1 0 0 0 0 0 0 

```

the above example is how you calculate and convert an IP Address in Binary and calculate it 

	tip1 : rememeber 128 64 32 16 8 4 2 1
	tip2 : remember to add the octets and match 
	them with the powers of base  
---
