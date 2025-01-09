+++
date = '2025-01-07T15:57:37+01:00'
draft = false
title = 'About'
+++

# Hi,
i'm a French person passionate about technology, IT and computers in general.
I love tinkering with servers, Linux in general, Rimworld, Cyberpunk 2077 and cats.<br>
I personnaly own a Poweredge T320 & a custom built NAS

# Computers Details
### Main desktop
- Ryzen 5 3600
- 48gb DDR4 2666MHz
- RX 5500XT (Main GPU)
- GTX 1660 SUPER (to passthrough inside VMs)
- 1tb NVMe
- 1tb HDD
- oh, and I use arch btw

Why passing a GPU to a VM ? mostly because I do music stuffs, and I don't like Linux DAWs at all <sub><sup>and I already bought an FL Studio licence :)<br>
**(support developers if you love their products, especially if they offer lifetime update when every others don't ;)** <br><br></sub></sup>
And because it's very nice to have smooth VMs, I started using more with GPU, some to record videos, others to browse / use certains apps with VPNs (I find it easier to do "split-tunneling" that way instead of tinkering with **iptables**)

### Macbook - M1 Pro
- 16gb RAM
- 500gb SSD

I use it when I travel (almost never) and to test apps & stuff.<br>
Before I bought a 2nd GPU, it was my main music production device.

# Servers details:
### Poweredge T320
- Intel Xeon E5-2420 v2 @ 2.20GHz
- 32GB DDR3
- 4 x 3tb SAS HDD *(7k rpm)*
  - for data and backups, and I also seed Linux ISOs. Having OS, Docker and programs on a different HDD pool allows faster I/O performance for both the system and the file operations.
  - RAID 5, approximately 9tb avail.
- 2 x 300gb SAS HDD *(15k rpm)*
  - mainly for OS & programs, I watched some performance tests, IIRC two 15k HDD are not much slower compared to SATA SSDs
  - RAID 0

This is my main server. I use it for backups, torrents, NAS, Docker... therefore it handles my 20+ container very well and it almost never reach half of CPU usage.<br><br>
One reason I switched my apps from my NAS to this box is the price of SAS disks compared to SATA, for the price of 12tb of capacity (SAS, used), I could only buy 6tb of capacity (SATA, also used)<br>
Anyways, I am very happy about it, yet It draws quite a bit of energy
  
### Custom NAS
- Intel Core i7 6700
- 16gb DDR4 *(I previously had 32 but two sticks died)*
- 2 x (2 x 1tb SATA HDD) including one that is dead
  - That was my first NAS, awful at every level. Main pool is degraded, the case is the cheapest on Amazon, so disks are lying inside on top of each others, one pool (SSD) contains just one disk and the remaining of the RAM is dying. Oh, and every part was bought used so two motherboards died until now :)
  - two RAID 1 pools (~ 2tb avail.)
- 1 SDD - 500gb
  - It was mainly used for apps, now it's used as a fast network share as I don't have any other SSD on any of my other servers.
  
The only reason I still don't disconnect this monstruosity is Plex. I have no other GPU or CPU to replace the Core i7 for video transcoding. I think I will tranform it to a genuine Plex Box when I have enough money to buy at least two pair of HDD and a proper case.
