---
created: 2025-07-04T18:51:00
tags:
  - diagram
  - fundamentals
  - learning
---
---




## 🖥️ A Setup of DHCP server 
### [DHCP Setup](screenshots/DHCP-setup.png)

* in the above setup , i included an intermediary device `switch`
  
* along with a server on the top , connected through copper cables 
  
* configured the `DHCP` in server by adding a class c range along with a google dns : `8.8.8.8` along with a gateway of `192.168.100.254`
  
	* the server will now assign the ip addresses to the `hosts` according to the configured IP range given to it 

---
