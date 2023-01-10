# 42-NetPractice
NetPractice is a general practical exercise to let you discover networking.

The networks you will be working with in this project are not real networks. They will be accessible via a training interface that you open in your web browser.

Only IPv4 addresses are used in NetPractice.
<!--
### What are TCP/IP addresses and how do they work?
```     
- TCP/IP, in full Transmission Control Protocol/Internet Protocol,
  standard Internet communications protocols that allow digital computers 
  to communicate over long distances.
        
- TCP guarantees the integrity of the data being communicated over a network.
  Before it transmits data, TCP establishes a connection between a source and 
  its destination, which remains active until communication begins. 
  It then breaks large amounts of data into smaller packets,
  while ensuring end-to-end delivery without loss of any data.
        
```
-->
<img width="1000" alt="Preamble" src="https://user-images.githubusercontent.com/97880185/211422027-874250ac-aac1-4100-a5ae-dab275c34c31.png"> <br />
<br />
### What are TCP/IP addresses and how do they work?
```     
- TCP/IP, in full Transmission Control Protocol/Internet Protocol,
  standard Internet communications protocols that allow digital computers to 
  communicate over long distances. 
```
### What is Transmission Control Protocol
```
- TCP guarantees the integrity of the data being communicated over a network.
  Before it transmits data, 
  TCP establishes a connection between a source and its destination,
  which remains active until communication begins. 
  It then breaks large amounts of data into smaller packets,
  while ensuring end-to-end delivery without loss of any data.
    
- TCP (Transmission Control Protocol) is a protocol that allows communication 
  between computers to be carried out in small packets and lossless. In fact,
  the most important feature of the TCP (Transmission Control Protocol) 
  protocol is that it performs the authentication and execution of the data 
  when sending or receiving data from the other party. 
  The TCP protocol was written to hide the losses that occur in 
  advanced computer networks.
```
### What is IP address
```
- IP addresses are the addresses required to connect to the internet.
  It is not possible for your device using the internet without an 
  IP address to connect to the internet.
  Thanks to IP addresses, computers find each other and perform data flow.
  Public IP and private IP addresses are used for this.
```
### IP address
</br>
<p align="center">
  <img width="388" alt="388-321" src="https://user-images.githubusercontent.com/97880185/211622199-e08ab318-5964-4db3-af73-0df9475868af.png">
</p>

### What is a Public IP Address?
```
- The IP address that allows two computers to recognize each other is 
  called a public IP address.
  A public IP address is usually used to access the Internet. 
  With a public IP address,
  you can access your computer or other electronic devices remotely.
```
### Public IP address ranges
```
- 1 IP address can have up to 255 values.
- Returns to 0 after 255.

. 0 (binary: 00000000)
. 1 (binary: 00000001)
. 2 (binary: 00000010)
. 3 (binary: 00000011)
. ...
. ...
. ...
. 252 (binary: 11111100)
. 253 (binary: 11111101)
. 254 (binary: 11111110)
. 255 (binary: 11111111)

BINARY  | 0000000 - 1111111
DECIMAL | 0 - 127

- For example
             IP address | 104.198.241.125
             IP address | 01101000.11000110.11110001.01111101

- Public IP addresses cannot take values from private IP addresses, 
  they only take values different from private IP address values.
```
### What is a Private IP Address?
```
- The IP address that several devices create when they are connected to 
  each other wired or wirelessly is called a private IP address.
  Devices on this network are not assigned the same IP address.
  Each is assigned a different IP address and these IP addresses 
  cannot be repeated.
  Computers on different networks can use the same addresses.
  It's okay if they use the same address since they're on different networks.
  There is also an incentive to use private IP addresses to save data.
  With private IP addresses, 
  it is not possible to route or stream data from the internet.
  The assignment of these addresses is also not controlled by anyone.
```
### Private IP address ranges
`10.0.0.0    – 10.255.255.255 `<br>
`172.16.0.0  – 172.31.255.255 `<br>
`192.168.0.0 – 192.168.255.255`<br>
`127.0.0.0   – 127.255.255.255`
### What is IP masking
```
- In TCP/IP, two devices can tell if they are on the same network by looking 
  at the first few digits of each other's IP addresses. 
  This step is called the IP mask or Subnet mask (IP mask or Subnet Mask). 
  For example, if the IP mask is 255.255.255.0, two machines 
  with the same first three digits (ie first 24 bits) are on the same network. 
  In this case, 192.168.0.1 and 192.168.0.2 are on the same network, and 
  192.168.1.1 is on another network.
  
  
***
- DECIMAL
        IP address | 104.198.241.125
        Mask       | 255.255.255.128
  
- BINARY
        IP address | 01101000.11000110.11110001.01111101
        Mask       | 11111111.11111111.11111111.10000000
```
### Masking example
</br>
<p align="center">
  <img width="389" alt="Mask" src="https://user-images.githubusercontent.com/97880185/211624489-1083a254-6f38-4aaa-866c-75d2d7092de6.png">
</p>

### Connection switch
```
- A switch connects multiple devices together in a single network. 
  Unlike a router, the switch does not have any interfaces since it only 
  distributes packets to its local network, 
  and cannot talk directly to a network outside of its own.
```

### Key example
</br>
<p align="center">
  <img width="389" alt="key" src="https://user-images.githubusercontent.com/97880185/211623839-3220c7ec-70da-49c7-a7c8-4ff54d877b6d.png">
</p>

### Router
```
- Just as the switch connects multiple devices on a single network, 
  the router connects multiple networks together. 
  The router has an interface for each network it connects to.

- Since the router separates different networks, 
  the range of possible IP addresses on one of its interfaces must 
  not overlap with the range of its other interfaces. An overlap in the 
  IP address range would imply that the interfaces are on the same network.
```
### Router example
</br>
<p align="center">
  <img width="400" alt="Router" src="https://user-images.githubusercontent.com/97880185/211625628-45dff831-f562-4934-b6ab-701dde3d5263.png">
</p>

### 10 questions in total
<details>
  <summary>Level 1</summary>
  <br>
  <img src="https://github.com/
  <br>
  <br>
 Here we have two separate networks, each consisting of two computers.<br>
  In order to make it work, the two computers need to be part of the same network.<br>
  Because the mask of A and B is `255.255.255.0` the possible IP-adresses of A1 are <br>`104.99.23.1 - 104.99.23.254`.<br>
  For C and D the mask is `255.255.0.0`, so the usable IP's are `211.191.0.1 - 211.191.255.254`

  <br>
  <br>

  <br>
  <br>
  
  <br>
  <br>

  <br>
  <br>


  <div align="right">
  <b><a href="#top">↥ back to top</a></b>
</div>
</br>

</details>

-------

<details>
<summary>Level 1</summary>
<br>
<img src="https://github.com
<br>
<br>
```
- Here we have two separate networks, each consisting of two computers.
  In order to make it work, the two computers need to be part of the same network.
  Because the mask of A and B is `255.255.255.0` the possible 
  IP-adresses of A1 are <br>`104.99.23.1 - 104.99.23.254`.
  For C and D the mask is `255.255.0.0`, 
  so the usable IP's are `211.191.0.1 - 211.191.255.254`
```
  <br>
  <br>

  <br>
  <br>
  
  <br>
  <br>

  <br>
  <br>


  <div align="right">
  <b><a href="#top">↥ back to top</a></b>
</div>
</br>

</details>
                   
-----

<details>
  <summary>Level 1</summary>
  <br>
  <img src="https://github.com
  <br>
  <br>
 Here we have two separate networks, each consisting of two computers.<br>
  In order to make it work, the two computers need to be part of the same network.<br>
  Because the mask of A and B is `255.255.255.0` the possible IP-adresses of A1 are <br>`104.99.23.1 - 104.99.23.254`.<br>
  For C and D the mask is `255.255.0.0`, so the usable IP's are `211.191.0.1 - 211.191.255.254`

  <br>
  <br>

  <br>
  <br>
  
  <br>
  <br>

  <br>
  <br>


  <div align="right">
  <b><a href="#top">↥ back to top</a></b>
</div>
</br>

</details>

<details>
  <summary>Level 1</summary>
  <br>
  <img src="https://github.com
  <br>
  <br>
 Here we have two separate networks, each consisting of two computers.<br>
  In order to make it work, the two computers need to be part of the same network.<br>
  Because the mask of A and B is `255.255.255.0` the possible IP-adresses of A1 are <br>`104.99.23.1 - 104.99.23.254`.<br>
  For C and D the mask is `255.255.0.0`, so the usable IP's are `211.191.0.1 - 211.191.255.254`

  <br>
  <br>

  <br>
  <br>
  
  <br>
  <br>

  <br>
  <br>


  <div align="right">
  <b><a href="#top">↥ back to top</a></b>
</div>
</br>

</details>

<details>
  <summary>Level 1</summary>
  <br>
  <img src="https://github.com
  <br>
  <br>
 Here we have two separate networks, each consisting of two computers.<br>
  In order to make it work, the two computers need to be part of the same network.<br>
  Because the mask of A and B is `255.255.255.0` the possible IP-adresses of A1 are <br>`104.99.23.1 - 104.99.23.254`.<br>
  For C and D the mask is `255.255.0.0`, so the usable IP's are `211.191.0.1 - 211.191.255.254`

  <br>
  <br>

  <br>
  <br>
  
  <br>
  <br>

  <br>
  <br>


  <div align="right">
  <b><a href="#top">↥ back to top</a></b>
</div>
</br>

</details>

<details>
  <summary>Level 1</summary>
  <br>
  <img src="https://github.com
  <br>
  <br>
 Here we have two separate networks, each consisting of two computers.<br>
  In order to make it work, the two computers need to be part of the same network.<br>
  Because the mask of A and B is `255.255.255.0` the possible IP-adresses of A1 are <br>`104.99.23.1 - 104.99.23.254`.<br>
  For C and D the mask is `255.255.0.0`, so the usable IP's are `211.191.0.1 - 211.191.255.254`

  <br>
  <br>

  <br>
  <br>
  
  <br>
  <br>

  <br>
  <br>


  <div align="right">
  <b><a href="#top">↥ back to top</a></b>
</div>
</br>

</details>

<details>
  <summary>Level 1</summary>
  <br>
  <img src="https://github.com
  <br>
  <br>
 Here we have two separate networks, each consisting of two computers.<br>
  In order to make it work, the two computers need to be part of the same network.<br>
  Because the mask of A and B is `255.255.255.0` the possible IP-adresses of A1 are <br>`104.99.23.1 - 104.99.23.254`.<br>
  For C and D the mask is `255.255.0.0`, so the usable IP's are `211.191.0.1 - 211.191.255.254`

  <br>
  <br>

  <br>
  <br>
  
  <br>
  <br>

  <br>
  <br>


  <div align="right">
  <b><a href="#top">↥ back to top</a></b>
</div>
</br>

</details>

<details>
  <summary>Level 1</summary>
  <br>
  <img src="https://github.com
  <br>
  <br>
 Here we have two separate networks, each consisting of two computers.<br>
  In order to make it work, the two computers need to be part of the same network.<br>
  Because the mask of A and B is `255.255.255.0` the possible IP-adresses of A1 are <br>`104.99.23.1 - 104.99.23.254`.<br>
  For C and D the mask is `255.255.0.0`, so the usable IP's are `211.191.0.1 - 211.191.255.254`

  <br>
  <br>

  <br>
  <br>
  
  <br>
  <br>

  <br>
  <br>


  <div align="right">
  <b><a href="#top">↥ back to top</a></b>
</div>
</br>

</details>
<details>
  <summary>Level 1</summary>
  <br>
  <img src="https://github.com
  <br>
  <br>
 Here we have two separate networks, each consisting of two computers.<br>
  In order to make it work, the two computers need to be part of the same network.<br>
  Because the mask of A and B is `255.255.255.0` the possible IP-adresses of A1 are <br>`104.99.23.1 - 104.99.23.254`.<br>
  For C and D the mask is `255.255.0.0`, so the usable IP's are `211.191.0.1 - 211.191.255.254`

  <br>
  <br>

  <br>
  <br>
  
  <br>
  <br>

  <br>
  <br>


  <div align="right">
  <b><a href="#top">↥ back to top</a></b>
</div>
</br>

</details>

<details>
  <summary>Level 1</summary>
  <br>
  <img src="https://github.com
  <br>
  <br>
 Here we have two separate networks, each consisting of two computers.<br>
  In order to make it work, the two computers need to be part of the same network.<br>
  Because the mask of A and B is `255.255.255.0` the possible IP-adresses of A1 are <br>`104.99.23.1 - 104.99.23.254`.<br>
  For C and D the mask is `255.255.0.0`, so the usable IP's are `211.191.0.1 - 211.191.255.254`

  <br>
  <br>

  <br>
  <br>
  
  <br>
  <br>

  <br>
  <br>


  <div align="right">
  <b><a href="#top">↥ back to top</a></b>
</div>
</br>

</details>


























<!--
### This interface should open in your web browser; <br />
<img width="800" alt="web" src="https://user-images.githubusercontent.com/97880185/211425347-0cd650b3-ed4e-4a09-9e16-0b27d0b73cbf.png">
<img width="800" alt="web2" src="https://user-images.githubusercontent.com/97880185/211425214-b0166390-b9fe-4fbf-aa7a-2c1ad83e2a7b.png">
-->
