# 42-NetPractice
NetPractice is a general practical exercise to let you discover networking.

The networks you will be working with in this project are not real networks. They will be accessible via a training interface that you open in your web browser.

Only IPv4 addresses are used in NetPractice.

</br>
<p align="center">
  <img width="800" alt="ETHERNET CABLE" src="https://user-images.githubusercontent.com/97880185/211422027-874250ac-aac1-4100-a5ae-dab275c34c31.png">
</p>

<p align="center">
  <img width="150" alt="Host" src="https://user-images.githubusercontent.com/97880185/211656437-609c2afe-8673-4b69-b960-9a8247a855c3.png">
  <img width="150" alt="Router" src="https://user-images.githubusercontent.com/97880185/211656451-11235c84-f555-427b-916e-93a428a816b9.png">
  <img width="150" alt="Switch" src="https://user-images.githubusercontent.com/97880185/211656464-3daa6f82-578b-4c6b-8d54-ff28b93e670f.png">
  <img width="130" alt="Internet" src="https://user-images.githubusercontent.com/97880185/211656370-91ad141f-d7c5-4877-8136-0f7f6237c646.png">
</p>
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
### Masking-example
</br>
<p align="center">
  <img width="389" alt="Mask" src="https://user-images.githubusercontent.com/97880185/211624489-1083a254-6f38-4aaa-866c-75d2d7092de6.png">
</p>

### Connection-switch
```
- A switch connects multiple devices together in a single network. 
  Unlike a router, the switch does not have any interfaces since it only 
  distributes packets to its local network, 
  and cannot talk directly to a network outside of its own.
```

### Key-example
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
### Router-example
</br>
<p align="center">
  <img width="400" alt="Router" src="https://user-images.githubusercontent.com/97880185/211625628-45dff831-f562-4934-b6ab-701dde3d5263.png">
</p>






























<!--
### 10 questions in total
<details>
  <summary>Level 1</summary>
  <br>
  <img src="https://github.com/"
  <br>
  <br>
  Here we have two separate networks, each consisting of two computers. <br>
  In order to make it work, the two computers need to be part of the same network. <br>
  Because the mask of A and B is `255.255.255.0` the possible IP-adresses of A1 are <br>`104.99.23.1 - 104.99.23.254`. <br>
  For C and D the mask is `255.255.0.0`, so the usable IP's are `211.191.0.1 - 211.191.255.254`.
  
  
</details>

---
<details>
  <summary>Level 2</summary>
  <br>
  <img src="https://github.com/"
  <br>
  <br>
  Here we have two separate networks again, but this time we need to set the mask and IP correctly.<br>
  For the network of A and B, they need the same mask, `255.255.255.224`.<br>
  The available IP-addresses for A1 are `192.168.57.193 - 192.168.57.221`.<br>


  Network C and D already has the same mask. so they just need addresses that are part of the same subnet.<br>
  In the case of the mask beeing `/30` the subnet only consists of 2 available addresses per subnet.<br>
  So be carefull, to choose the correct ones. to make things easier,<br>
  i suggest you either start with the lowest or highest subnet.<br>
  I choose the highest, so my available IP-range is `192.168.57.253 - 192.168.57.254`
  
</details>

---
<details>
  <summary>Level 3</summary>
  <br>
  <img src="https://github.com/"
  <br>
  <br>
  In this level we have our first encounter with a [Key example](https://github.com/farukdll/42-NetPractice#Key-example).<br>
  Since we can't manipulate the mask of C, `255.255.255.128` will be the mask of the whole network.<br>
  A has a fix IP, so the whole networks range will be `104.198.187.1 - 104.198.187.126`.
  
</details>

---
<details>
  <summary>Level 4</summary>
  <br>
  <img src="https://github.com/"
  <br>
  <br>
  This is our first time running into a router, since the router does not connect to anything else,<br>
  there is no routing table, that needs to be worked with.<br>
  A has a fixed IP, so this will define the IP of our network.<br>
  You can freely choose a fitting mask for the network, but the subnet has to have at least 3 usable IP-addresses, <br> 
  so choosing `255.255.255.240`/`/28` will create a subnet of 14 usable addresses.<br>
  The fixed IP of A is `67.52.110.132`.<br>
  This results in a available IP-range of `67.52.110.129 - 67.52.110.142`.
  
</details>

---
<details>
  <summary>Level 5</summary>
  <br>
  <img src="https://github.com/"
  <br>
  <br>
  Here we first come by the mighty routing table.<br>
  R1 has a fixed IP of `80.103.79.126` and a fixed mask of `255.255.255.128`, <br>
  which results in a mask of `255.255.255.128` and an IP-range of `80.103.79.1 - 80.103.79.125` for A1.
  
  
  Now to conquer the routing table of A it is as easy as setting the **destination** as `default` <br> 
  or `0.0.0.0/0` and the destination has to be the IP of the directly connected router R1, `80.103.79.126`.<br>
  
</details>

---
<details>
  <summary>Level 6</summary>
  <br>
  <img src="https://github.com/"
  <br>
  <br>
  This level introduces us to the Internet.<br>
  We again start with looking at the fixed IP-addresses and masks.


  IP of A1 is fixed and mask of R1, which A1 is connected to through the switch, is fixed as well.<br>
  So we need to match those in order for them to be in the same network.<br>
  Mask for this network will be `255.255.255.128` which then will result in 2 subnets.<br>
  Combined with the fixed IP of `29.65.6.227` one subnet will be from `29.65.6.1` to `29.65.6.126` and <br>
  the other <br>`29.65.6.129 - 29.65.6.254`.<br>
  In order for R1 and A1 to be in the same network, the possible address-range of R1 will be `29.65.6.129 - 29.65.6.254`.
  
  Now set the routing table of A in order to reach R1.


  The **destination** of the routing table of the internet needs to be set to the network address <br> 
  of the R1-A1 network, which in this case is `29.65.6.128`, combined with the CIDR of the network, which is `/25`.<br>
  This results in a **next hop** of `29.65.6.128/25`.


  **Destination** of the routing table of the router can be set to `default` or `0.0.0.0/0`.
  
</details>

---
<details>
  <summary>Level 7</summary>
  <br>
  <img src="https://github.com/"
  <br>
  <br>
  Level 7 is pretty straight forward and not too complicated, you just need to make sure that no networks overlap with each other.
  
  First goal will be to find an appropriate mask to use.<br>

  - A1 R11 (network range of `107.198.14.0 - 107.198.14.3`)
  - R12 R21 (network range of `107.198.14.252 - 107.198.14.255`)
  - R22 C1 (I did choose a network range of `107.198.14.4 - 107.198.14.7`)
  
</details>

---
<details>
  <summary>Level 8</summary>
  <br>
  <img src="https://github.com/"
  <br>
  <br>
  Level 8 now will be a little tricky because you really need to be aware of overlapping networks.


  First thing we can solve is the connection of R13 and R21.<br>
  The routing table of R2 gives you the fixed IP of R13 as `141.195.172.62` and as this network only <br> 
  consists of 2 needed IP-addresses we can set the mask of R13 and R21 to `255.255.255.252` in order to make <br>
  things easier with overlapping IP-addresses.<br>
  Then this will result in `141.195.172.61` as the address of R21.<br>

  In R12 we see the fixed IP, which is `163.166.250.12`, so this needs to be put into the routing table of the Internet.<br>

  Now to set up the connection of D1 and R23.<br>
  First, set the mask of R23, since the mask of D1 is fixed to `255.255.255.240`.<br>
  Then put in 2 IP-addresses which are part of the same network intoR23 and D1, <br>
  I decided to use the lowest subnet of the mask, since it is a not used IP-range yet, <br>
  which is `141.195.172.1 - 141.195.172.14`.<br>
  So IP of R23 will be `141.195.172.1` and of D1 will be `141.195.172.2`.<br>


  For the network between R22 and C1 we are free to choose any mask we want. <br>
  In order to make it as easy as possible I set it to `255.255.255.252`, <br>
  because I only need 2 usable IP-addresses. After that I then choose a free range for my IP's.<br>
  In this case I did chose the next free one after the network of R23 and D1, which will be `141.195.172.17 - 141.195.172.18`.<br>


  Last thing to do is to set all the routing tables accordingly.<br>
  For C and D it's easy, both use `default` or `0.0.0.0/0` as a **destination** and the IP of the Interface of R2 they are directly connected to as **next hop**.<br>

  For the routing table of R1 it is a little harder.<br>
  Even though it would, for Net_Practice, work to just set the **destination** to `default` and get away with it just working, <br>
  there is no way this should work as easy as this.<br>
  Because that would result in the routing table having 2 default destinations which lead to a different **next hop**, <br>
  which if you think about doesn't make any sense, because the router would have no way of knowing which default to use.


  To make it more sensible, the destination needs to be set to a value that leads to R2 and can go either way,<br>
  to D1 and to C1. Because we used the lowest two IP-ranges for the two target networks, <br>
  that need to be reached, the **destination** will be `141.195.172.0/27` the IP adress is of the network, <br>
  that we want to reach and the CIDR will just define that the first 27 bits of the IP have to be `141.195.172`, <br>
  so it will be able to communicate with IP's ranging from `141.195.172.0` to `141.195.172.255`.

</details>

---
<details>
  <summary>Level 9</summary>
  <br>
  <img src="https://github.com/"
  <br>
  <br>
  In Level 9 we encounter another weakness of the project. The router is not doing any IP-translation when a computer reaches out to the internet.<br>
  This can be seen by trying to connect C to the internet.


  First we set the ,mask of R22 and C1 to `255.255.255.252`, in order to block as little IP's as possible.<br>
  Now you have to decide on which IP-range to use for this network. I decided for the top-end, with the usable IP-addresses beeing `10.0.0.253` and `10.0.0.254`.<br>
  Now set the **next hop** in the routing table of C to the IP of R22.<br>
  Now change the routing table of R1, R2 and the Internet to make it work, as you learned before.


  If you now hit the `check again` button, it will show you `Goal 6 : cation need to communicate with Internet - Status : KO - No reverse way, try again ...` for this demonstration we will just ignore all of the other goals.<br>
  Now you can see at the small red box at the bottom right corner:

  ```
  ******* Goal ID 6 ********
  forward way : C -> I (163.172.250.1)
  on C : packet accepted
  on C : destination does not match any interface. pass through routing table
  on C : route match 0.0.0.0/0
  on C : send to gateway 10.0.0.254 through interface C1
  on R2 : packet accepted
  on R2 : destination does not match any interface. pass through routing table
  on R2 : route match 0.0.0.0/0
  on R2 : send to gateway 50.165.17.254 through interface R21
  on R1 : packet accepted
  on R1 : send to R12
  on I : packet accepted
  on I : destination reached
  reverse way : I -> C (10.0.0.253)
  on I : packet accepted
  private subnets not routed over internet
  ```

  From this we can see, the package from C reaches the Internet, but since the router only attached the private IP of C1 without translating it to a public IP, the Internet can't send any package back to a private IP.<br>


  All we have to do now to make it work, is to change every apperance of our `10.0.0.x` address to `9.0.0.x`.<br>
  Once you have done that you are greeted with <br>`Goal 6 : cation need to communicate with Internet - Status : OK - Congratulations !!`


  So, for Net_Practice, a network can't have any IP which is part of a private Network, as soon as it will need connection to the Internet.


  Now, all that is left is to solve the remaining 5 Goals.


  3 Goals will be solved by creating the A-B-R11 network first, then connecting it to the Internet.<br>
  First, the mask of R11 is fixed, so set the same for B1 and A1.<br>
  Second, this network can not use private IP-addresses, so get rid of them.<br>
  Third, set the routing tables of A and B so they can reach R11.<br>
  Fourth, set the network address combined with the mask as a **destination** in the routing table of the internet.<br>
  In my case this was `106.198.154.0/25`.<br>


  The last two goals are depending on D to work.<br>
  As you can see in the routing table of D, the **next hop** is fixed, so put the same IP into R23.<br>
  The **destination** can be set to `default` or `0.0.0.0/0`.<br>
  Since the mask of that network is fixed as well, set it accordingly.


  Now, if we didn't forget anything, all that should be left, is to fix the routing table of R1.<br>
  For this you need the network-address of the R23-D1 network.<br>
  You can find this with the same logic, as before by just extending the [table](https://github.com/tblaase/Net_Practice#masks) above.<br>
  With this you will be able to find out that the mask `/18` divides our IP-range into 4 subnets:


  - `63.239.0.0 - 63.239.63.255`
  - `63.239.64.0 - 63.239.127.255`
  - `63.239.128.0 - 63.239.191.255`
  - `63.239.192.0 - 63.239.255.255`


Our fixed IP is part of `63.239.64.0 - 63.239.127.255`, so the network-address is `63.239.64.0`, combine this with our mask of `/18` and you have the missing **destinaton** of our routing table, `63.239.64.0/18`.

  
</details>

---
<details>
  <summary>Level 10</summary>
  <br>
  <img src="https://github.com/"
  <br>
  <br>
  The easiest part will be the connection of H2 and H1 in their network.<br>
  The mask of this network is fixed by R11, set the masks of H21 and H11 accordingly.<br>
  Set the IP of H21 to match the rest of the network, it can be in the range of `158.103.36.3 - 158.103.36.126`.<br>

  Now we are setting up the H41-R23 network and its connection to the Internet.<br>
  The mask is fixed, so set it accordingly.<br>
  The IP of R23 is fixed by the routing table of H4, so set it to the correct one.<br>
  Now go along the route connecting it to the Internet, you will notice the mask of R21 is fixed so set the mask of R13 accordingly.<br>
  The routing table of R1 already has the default set, as a connection to the internet.<br>
  So now the package should be able to reach the Internet and only thing to fix is the routing table of the Internet.<br>
  For this to be correct we only need to change the CIDR of the **destination**, so it is able to communicate with all `158.103.36.x` addresses.<br>
  This is done by changing the CIDR to `/24`, so it can reach `158.103.36.0 - 158.103.36.255`.<br>


  The hardest part of this level will now be the setup of the R22-H31 network and the correct setup of the routing table of R1.<br>
  First, set the mask of R22 and H31 to `255.255.255.252` since we only need 2 usable IP-addresses and this creates the least problems with overlapping ip-ranges.<br>
  Second, you need an IP-range that is still free. For this, we will take a look at all of the other networks.<br>


  - `150.152.40.0 - 150.152.40.127` is taken by R11-H21-H11
  - `150.152.40.128 - 150.152.40.191` is taken by R23-H41
  - `150.152.40.252 - 150.152.40.255` is taken by R13-R21


  So my decision was to take the next free part after `150.152.40.128 - 150.152.40.191`, which with the `/30` mask will be `150.152.40.192 - 150.152.40.195`.<br>
  Set the addresses accordingly to the usable ones of the range, you decided on.<br>


  Lastly, for the routing table of R1 we need the network-address of the R22-H31 network, which in my case is `150.152.40.192/` and it's mask, which is `/30`, set the **destination** accordingly.<br>
  
</details>

---
-->

























<!--
### This interface should open in your web browser; <br />
<img width="800" alt="web" src="https://user-images.githubusercontent.com/97880185/211425347-0cd650b3-ed4e-4a09-9e16-0b27d0b73cbf.png">
<img width="800" alt="web2" src="https://user-images.githubusercontent.com/97880185/211425214-b0166390-b9fe-4fbf-aa7a-2c1ad83e2a7b.png">
-->
