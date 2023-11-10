---
layout: page
title: About
permalink: /about/
---  
## _"**Slim Reaper** is my name and labbing is my game"_  

 &nbsp; &nbsp; &nbsp; &nbsp; I am a tinkerer by nature. My journey began with Diablo 2. My borther and I used to visit gaming centers in Bakerfield,CA (where we grew up). After a while the money added up. Our cousins neighbor had built their own "rig" and, we instantly want to do the same. So the begging bagan. My mom is a big supporter ours and has always been willing to sink large amounts of funds into whatever hobby had piqued our interest. Otherwise we would have been out of luck. So we set off to the now non-existant **_Compusa_** store to purchase parts for our build. The rest is history. From there I began to tinker with building html and css sites and trying to learn to code. I quickly realized my interests lied more heavily with hardware and networking. Fast forward 15 years later I began building this lab.  

&nbsp; &nbsp; &nbsp; &nbsp; I really got serious about labbing around 2 years ago. Prior to that I was purely interested in tech from an entertainment standpoint. It was fun to use and allowed me to play games with great graphics and awesome FPS. I am not really sure why but I began to want to learn to be a hacker. Purely for educational research and not with mal-intent. As I began to play with Kali Linux and metasploit, HACKTHEBOX, TRYHACKME, etc. I quickly realized the limitations of my knowledge and began from square one. I picked up some comptia books and perused the inter-web on forums to obsorb as much knowledge as I could. I needed to the know more than just surface level. I wanted to know why something worked and in what order it worked. If I could grasp that then I could understand how to break them. Most of my projects seem to the begin that way.  

&nbsp; &nbsp; &nbsp; &nbsp; Once I started to get a grasp of networking and servers I purchased my first 1u server and all the required additions _(UPS, Rack, etc)_ along with my first fully configurable layer 3 switch. I had a raspberry pi 3b+ already from a previous holiday gift and I was off and running. I loaded proxmox on the 1u server, updated the fireware on the HP Procurve switch, and hosted PI-Hole on the Rasp-Pi and began labbing. To be honest I did not have an exact IT role in mind when I bagan my lab. I took the kitchen sink approach and began learning all that I could. Ultimately I ended up make the 1u server a Windows Server 2019 enviornment with multiple Windows 10 Pro VM's. That was a lot of fun as I had never domain join a PC before nor had I set up a ADDC. It took me 4 tries of wiping and reinstalling before I was ultimately able to get the DC up and runnning and the VM's joining properly.  

&nbsp; &nbsp; &nbsp; &nbsp; Due to having a configuable switch I set off to learn as much about network segmentation, access control, logging, and CLI cofiguration that I could. Networking has been the steeepest learning curve. There are innumerable ways to break a network and sometimes getting back in to fix it can be tricky. Fortunately I have a forgiving family, as I have knocked it out more times than I can count. The basic set up of my network is the following: 
 
 ### WAN 
 <br />
 1) Ziply fiber OPN -> <br /> 
 ### LAN  
 <br />
 2) RT1 : Netgear Nighthawk -> <br />
 3) RT2 : Netgear WAP 123 RT2 (Flashed to OpenwRT) bridged to port 1 of RT1  <br />
 4) SW1 : 5 port GbE + SFP Uplink (SFP Uplink to Mikrotik RB2011)  ->  <br />
 5) SW2 : Trendnet 24 port switch + 2 SFP+ uplink (LAGG to 10GbE switch) -> <br />
 6) SW3 : Trendnet 12 port 10gbE SFP+ Switch (LAGG from 24 port Trendnet) -> <br />
 7) SW4 : HP PRocurve 1910 24 port GbE + 2 SFP Uplink (LAGG to 10GbE Trendnet) <br />
 8) SW5 : Mikrotik RB2011 (From SW1 SFP Uplink) <br />    

 &nbsp; &nbsp; &nbsp; &nbsp; You may be asking why in the world I have 2 routers and 5 switches. You would be justified in ponering that descision. Well the answer ties back into the ever expanding lab statement that I made previously. As my knowledge base grew I wanted to play with different routers and switches. I would add a new network device and then reconfigure how my endpoints were segmented or connected. They each provide a different purpose and support to different types of endpoints. I have IOT devices, VOIP devices, servers, PC's, etc. As the amount and variety of device types grew and the traffic with it, I decided to implement all these devices instead of getting rid of them. Plus to be honest they look really cool all stacked in my lab. My main goal was to have 10GbE Fiber running to all servers and PC's in the lab for file transfers to and from my Truenas Scale server I only have 1Gbe Fiber on my WAN as anything higher than that in my area is quite expensive at the moment. But I would love to have 10Gbe Fiber extending from my LAN al lthe way through to my lan and get of the bottleneck. 

_**To Be Continued....**_




### Contact me

[reaperlabs.online@proton.me](mailto:reaperlabs.online@proton.me)
