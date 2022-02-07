## 1/2 Induvidual Task per Group

**List of Topics:**

1. How to realise a Layer-2 Network with VxLAN on top of a Layer-3 Wireguard tunnel
2. How to build a backup system for file from your machine to your server through a Wiregurad tunnel
3. How to stream your game running on your desktop machine to your laptop through a Wireguard tunnel
4. How to make you home NAS (NextCloud) securly accessible through a Wireguard tunnel
5. How to setup two Wireguard links between your desktop and OpenWrt server for fail over
6. How to make your smart home electricity accounting with MQTT accessible through a Wireguard tunnel

**Please choose your team topic and fill it here**

|  Team 	       |   Topic   |   Desktop machine   |  fixed IP v4 from Medienzentrum
| :-------------:| :-------: | :----------------:  | :------------------------------: 
| Arwed/Edgar    | 4         |       Raupi         |   172.16.163.10/16
| Amer/Manh      | 6         |       Pikacho       |   172.16.163.11/16
| Nils/Martin    | 3         |       Smogmog       |   172.16.163.12/16
| Valerius/Oliver| 5         |       Karpador      |   172.16.163.13/16
| Andi/Florian   | 2         |       Kleinstein    |   172.16.163.14/16     

**Re-Configure IPv4 of your Desktop machine**
- use the IPv4 adress in the table from Medienzentrum
- configure your IPv4 gateway as: 172.16.1.1
- configure your DNS to: 195.37.88.1


## 2/2 Common Task per Group: "Find the right cat!"

Your goal is to find the correct cat picture that corespondes to the hash value as content of a text file on a BananaPI Router on your desk.

Each group has a network setup on its desk consisting of your Desktop PC to which you should have remote access (tmate & wireguard). 
All PCs are equiped with a second network card, which is connected to a 5-port switch. 
The router is connected to an electrical plugbar (called NETIO PowerBox4KF) that can be controlled over the network and an routerboard, called BananaPI. 
The bananaPI is powered over the plugbar and powered off by default.

In order to find the correct cat picture, you have to:

- access your lab-PC from remote
- find out the IP addresses of you network card and the NETIO Powerbox. (e.g. use tools like nmap, tcpdump, ping ...)
- find a way to access the powerplug over the network connection from your desktop pc (See the manual for the NETIO Powerbox 4KF)
- switch all 4 power ports on - the BananaPI router will boot up. (See the manual for the NETIO Powerbox 4KF)
- find the ip adress of your new booted BananaPI and acess it via ssh (user=root, password = Manni2021!)
- find the textfile with the name "secret.txt"
- find the matching cat picture's sha256sum hash that corresponds to the content of your secret.txt

Record your findings, what tool did you use to find out the IP addresses? How did you connect to the plugbar and power on you BananaPI? 
On which port of the plugbar was your BananaPI? What's the name of your BananaPI?
Make a small sheet how you solved the problem, roughtly one page
