---
created: 2025-07-04T14:47:00
---
---
---
[ports example](screenshots/ports-eg.png)

##  🚢 PORTS Summarized
---
* Your browser knows what tabs you opened and which contains which *==link==*
* PORTS are very important for forming the connection even with a ==target==
* PORTS can establish connection with remote servers using different PORTS on you *local machine*
* means can run HTTP and HTTPS as well 
---
* Network connections are made between PORTS
* an Open Port listening on the server , randomly selects port on your *computer*
	* and then connects to it and forms connections , the above image is an example of it 
		* open port selects 4953 on your *local machine* and then forms connections to port 443 (website-dns) , 443 is an HTTPS port
---

## 🤯 Total PORTS and more
---
* every computer has total **`65535`** available ports 
	* however many of these are registered as *standard ports*

* # Services Ports
	* `http : 80`
	* `https : 443`
	* `windows NETBIOS : 139`
	* `SMB : 445`
		* in CTF settings these can be altered making them a appropriate enumeration targets
---


## ➡️Summarized Process 
---
> here we will understand a summarized process of PORT 

* ### Steps
	* you send the request using an [ Open Port ] to the URL (dns) of a website 
	* the request is directed by traffic toward their ==PORT==
	* the ==PORT== receives your request and uses an *Open port* from your machine to form connection to its port eg : `HTTPS : 443` a designated port
	* the web server then sends back the *requested data* ( like a webpage) to your browser

> keep revisiting this section to keep things clear as its easy to confuse oneself

>thing about a port as an entry or an exit , (source (you) --> destination(port) but you need entry point when you want to enter)
---



