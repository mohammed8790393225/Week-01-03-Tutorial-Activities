# Week-01-Tutorial-Activities
Task 1. View Your Computer Information
Details of the computer hardware and OS is provided below:

CPU details
 ![CPU details](https://user-images.githubusercontent.com/128876454/227858456-bc7e4922-3041-49d1-89fe-3f3130f8ac0b.png)

OS version
 ![OS version](https://user-images.githubusercontent.com/128876454/227858494-a3fe1535-90af-40b5-a497-3c0ee1111d30.png)

RAM
 ![RAM](https://user-images.githubusercontent.com/128876454/227858622-fe1de2e5-2522-48b1-bbc4-2099e93e04dc.png)

Disk information
 ![Disk](https://user-images.githubusercontent.com/128876454/227858634-8676c2e1-6c4c-4d0c-9ee0-72dd583896c1.png)

Component Name	Details or Size
CPU	AMD Ryzen 3 3250 with Radeon graphics, Number of cores -2, number of logical processor – 4, max clock speed - 2600
RAM	8589934592 Bytes
DISKS	256060514304 Bytes
OS Version	Windows 11 Home Single language

Task 2. Deploy Linux Web Server in VirtualBox
Installing virtual box
 
 ![1](https://user-images.githubusercontent.com/128876454/227858801-2775d6a0-206d-42c9-ba23-de3a7a653dea.png)
![2](https://user-images.githubusercontent.com/128876454/227858811-4f372e62-5f55-4c62-8639-2b21e64bc829.png)
![3](https://user-images.githubusercontent.com/128876454/227858813-5b6d0ca9-b9f8-4eee-92c2-07e64fa1b41e.png)

 
Deploying web server
 
 ![11](https://user-images.githubusercontent.com/128876454/227859191-ce28d8e9-1f0a-4dea-92a2-394906439506.png)
![12](https://user-images.githubusercontent.com/128876454/227859238-5889f7b3-547f-49c8-a564-56247d9d4a8b.png)

Ans.!

Boot Manager: GRUB boot loader 2.0.6.
Kernel: Linux Kernel 5.4.
Task 3. Browse to OpenWRT Websites
 ![31](https://user-images.githubusercontent.com/128876454/227859590-6bef8f44-3104-4f7b-a464-f3cfdf2508df.png)

Browsing management interface
 ![32](https://user-images.githubusercontent.com/128876454/227859599-1b8e918f-ad9f-42f7-928a-d1bf1abc05e9.png)

The details of information of OpenWRT system are provided below:
CPU: AMD Ryzen 3 3250U
RAM Size: 128MB
Disk Size: 14.6 MB
OS Version: Linux 5.4
Task 4. Practice Units and Prefixes
In this task, some calculations related to number systems has been performed. 
Task 5. Create GitHub Account
The creation of the Github account is shown below: 
 ![51](https://user-images.githubusercontent.com/128876454/227859659-e92ab43b-cd5b-4045-8fc9-4e366584570a.png)
 
 ![52](https://user-images.githubusercontent.com/128876454/227859653-28abd16e-bf95-406c-bdf7-c377add079f2.png)


 
Task 6. Create Microsoft Azure Account
 ![61](https://user-images.githubusercontent.com/128876454/227859708-50febddf-cbef-47d8-92a9-de3ad7db09b7.png)

 ![62](https://user-images.githubusercontent.com/128876454/227859815-834b6b40-2b9a-4635-828e-22a1452c4f80.png)

Task 7. Learning Reflection
One topic that I find challenging in the first week of a computer systems and applications course is understanding the concept of computer architecture and how different hardware components interact with each other to perform tasks. However, I also found difficult in browsing the OpenWRT website. 
To overcome this difficulty, I have revisit the lecture notes and slides, watch related online videos, and seek assistance from the tutor or classmates during tutorials. I also try to visualize the flow of information and data between different components using diagrams or animations to help them understand the concept better. Additionally, I have practiced working with the PowerShell commands to view computer hardware information and get hands-on experience with virtual machines like OpenWRT to apply the theoretical knowledge to practical scenarios.

# Week-02-Tutorial-Activities

Task 1: View your address
 ![1](https://user-images.githubusercontent.com/128876454/227860839-ae4cbcf2-adea-4384-941b-e3929e64cc04.png)

The above figure shows the IP address of all interfaces of my computer. 
Task 2: Ping Your local router
The command has been used to get the IP address of the local router is provided below:
Get-NetRoute | Where { $_.DestinationPrefix -eq '0.0.0.0/0' -and $_.RouteMetric -eq 0 } | Select NextHop
 ![2](https://user-images.githubusercontent.com/128876454/227860997-906bd4fe-4d5e-45a8-9062-f27261ac0001.png)

However, by using ipconfig command, it is possible to get the ip address of local router:
![21](https://user-images.githubusercontent.com/128876454/227861041-d17c1dfe-68fc-4d7e-a78b-fd3b2e3f546c.png)

 
Here, IP address of the local router is 192.168.1.1.
Ping test
 ![22](https://user-images.githubusercontent.com/128876454/227861073-3519e95d-e334-4dd5-9dff-d67c7da63fd7.png)

Minimum, maximum, and average delay between computer and local router:
Minimum delay = 118ms
Maximum delay = 149ms
Average delay = 135ms
Task 3: Ping your openWRT linux server
IP address of the openWRT Linux server
 ![3](https://user-images.githubusercontent.com/128876454/227861130-d44f8975-6f90-4e46-9063-9b1d5defde61.png)

Ping from host computer
 ![31](https://user-images.githubusercontent.com/128876454/227861144-e0a8f062-99bc-4039-b088-0c85fc4d179c.png)

Wireshark capture
 ![32](https://user-images.githubusercontent.com/128876454/227861164-213d529e-68dc-4506-a3ac-31b0e4a1627d.png)

From the above figure, it has been seen that the ping test between host computer and OpenWRT machine has been captured.
Task 4: Trace path through internet
Opening a glass tool to perform traceroute
 ![4](https://user-images.githubusercontent.com/128876454/227861467-6470882f-80b2-4620-9abd-13e1364ee246.png)

Identifying path for reaching google.com
 ![41](https://user-images.githubusercontent.com/128876454/227861496-6922483d-0d0d-4027-83e8-e7a44a004c6f.png)

Identifying path for reaching international destination
 ![42](https://user-images.githubusercontent.com/128876454/227861514-73979bc0-8465-4d1d-872f-49cccbe12aaf.png)

The above figure shows the trace route between host computer and London.ac.uk website. For this tracing, the following key information has been identified: 
•	The traceroute shows that the packets travel through multiple routers before reaching the destination.
•	The routers are located in different geographical locations, such as the United States, Europe, and Asia.
•	The delay between the source and destination varies between 20 ms to 300 ms.
•	The key information learned from tracing the path includes the physical locations of the routers, the ISPs that own them, and the approximate delay between each hop.
Factors that may impact or contribute to the delay in the Internet include network congestion, routing inefficiencies, physical distance between the source and destination, and the quality of the network infrastructure. These factors can vary greatly, especially when traversing different networks, leading to varying delays across the Internet.
Task 5: Draw a network diagram
 ![5](https://user-images.githubusercontent.com/128876454/227861569-f229ccc8-78bc-4b4e-b6df-708cdc023166.png)

Figure: Network Diagram
Task 6: Find addresses of a website
In this task, different types of addresses of multiple websites has been identified. For the identification of the addresses, PowerShell tool has been utilized. The identification of addresses are provided:
 
 ![6](https://user-images.githubusercontent.com/128876454/227861651-c757e38f-321a-4d3a-9546-42cb7c717e6c.png)

The above figure shows that both the IPv4 and IPv6 address of a website has been identified. However, from the yahoo.com, a list of IPv4 and IPv6 addresses has been identified. If any type of address of a website is not identified it can be said that the website works only on IPv4 address.   
Task 7: Home internet connection
Type of home network connection is wireless which is shown below:
 ![7](https://user-images.githubusercontent.com/128876454/227861698-cabe04cd-1404-4852-aee8-0e1b9344d324.png)

 
Data rates of my home network connection is shown in the following figure:
 
 ![71](https://user-images.githubusercontent.com/128876454/227861728-196e6f11-c069-4ee5-9bc8-cc70061a33eb.png)

Name of the ISP is GSL Networks. 
Download speed – 36.50 Mbps
Upload speed – 17.7 Mbps
However, for this task, a speed test has been performed on different times of a day. In different times of a day, different speed has been identified. 
Morning speed
 ![m](https://user-images.githubusercontent.com/128876454/227861876-247749e2-8e82-463d-8daf-2080da21b207.png)

 
Afternoon Speed
 ![a](https://user-images.githubusercontent.com/128876454/227861900-e025dd19-26a9-4ef9-a0da-1b980af14a57.png)

 
Night speed
 ![n](https://user-images.githubusercontent.com/128876454/227861922-b5e11fda-5912-445a-989d-34eeb872230d.png)

 
The performance of the speed test has been changed at different times due to network congestion, which can happen during peak usage hours when many people are using the Internet at the same time. In my home, I got highest speed during early morning whereas lowest speed during evening. Network congestion can cause slowdowns and delays, making it difficult to access websites, stream videos or perform other online activities.
Another factor that can impact the performance of the speed test is the number of devices connected to the network. In evening there are multiple devices are using the Internet simultaneously, so they will be sharing the available bandwidth, which can lead to slower Internet speeds.

# Week-03-Tutorial-Activities

Task 1: View ARP table
The ARP table of the primary physical interface on my computer is provided below:

 ![1](https://user-images.githubusercontent.com/128876454/227862732-1458b8a9-9a9e-4c0c-89e8-3084f47a0a1f.png)

When my PC communicate with other devices on your LAN by pinging them or accessing websites, my computer sends out an ARP request to learn the MAC address of the device with the corresponding IP address. If the device is on the same network segment as my computer and is powered on, it will respond to the ARP request with its MAC address, which my computer then stores in its ARP table.
As I continue to communicate with other devices on your LAN, the ARP table will change dynamically as new devices respond to ARP requests and previously learned MAC addresses expire from the table. This allows my computer to maintain an up-to-date mapping of IP addresses to MAC addresses for devices on the network.
The devices that are "Reachable" by my computer are the ones that have responded to an ARP request from your computer and have their MAC addresses stored in your computer's ARP table. These devices can be directly communicated with by my computer without having to go through a router or other network device.
Task 2: Analyse the ping packet capture
a.	Inspecting the packets
The Wireshark capture are provided below:
 
 ![21](https://user-images.githubusercontent.com/128876454/227862820-a5a5aaab-8dd5-4b6f-bac2-5763a41396c4.png)

In this captured packet, there are total of 11 packets where 8 packets are ICMP packet and 3 packets are ARP packet. The ICMP packet mainly the ping test between the host computer and OpenWRT Linux guest. The ICMP packet are echo reply and request where source IP is 192.168.56.1 and destination IP is 192.168.56.2:
 ![22](https://user-images.githubusercontent.com/128876454/227862864-ecd93c0f-a9bc-4f18-a06f-ab0f7e0ab0ba.png)

 
b.	Network diagram
 ![23](https://user-images.githubusercontent.com/128876454/227862956-fd7b26f9-8d35-43ec-8c62-2f7842522471.jpg)

 
c.	Purpose of ARP packets
ARP (Address Resolution Protocol) packets are used to resolve the MAC address of a device on a local network given its IP address. They are sent by a device that wants to communicate with another device on the network, but only knows the IP address of that device, not its MAC address. The ARP packet is sent to the broadcast MAC address, and the device with the matching IP address will respond with its MAC address. The ARP packet is sent by the device that wants to communicate, to all devices on the network.
Here, ARP packet is sent by the windows host to known the MAC access of the OpenWRT Linux. 
d.	Packet diagram
 ![24](https://user-images.githubusercontent.com/128876454/227863003-ebb39146-aae8-48ff-8880-53ae2e956fa7.jpg)

 
e.	Explaining the first two ICMP packets
 
 ![25](https://user-images.githubusercontent.com/128876454/227863052-bd7a19a5-0821-4d8a-82aa-b395ee3ec27c.png)

The first two ICMP packets are echo requests and echo replies, which are used by the ping utility to test network connectivity between two devices. Here, the echo request are sent by windows host with 192.168.56.1 IP address and echo reply has been provided by OpenWRT Linux machine with 192.168.56.2 IP address. 
f.	Packet diagram for ICMP packet
 
 ![26](https://user-images.githubusercontent.com/128876454/227863090-b458e0a2-8ac1-4a36-acd4-3c16f3f9c484.png)

Task 3: Design a small network
a.	Network design
 ![3](https://user-images.githubusercontent.com/128876454/227863283-3a4f86ae-84e9-4516-afa3-ca63cfe86c19.png)

b.	Explanation on the design
The above figure shows the network design of my friend’s home. Here, a star topology has been followed to design. This topology provides easy management, scalability, and fault tolerance. Here, a switch has been utilized that supports PoE. The switch have enough ports to accommodate all the cameras. However, two VLANs have been created, one for the older cameras and one for the newer cameras. This will ensure that the video streams are segregated and prevent network congestion. The network design has been chosen because, it is easy to install and it provides better security. 
c.	Listing of equipment
In order to design the network, the following equipment’s are needed to be purchased:
Equipment Name	Quantity
Router	1
PoE Switch with atleast 12 ports	1
PoE Security Camera	6
NVR	1
Cables 	20

d.	Calculation of throughput
For the older cameras: 4 cameras x 720p x 10 fps x 50 (MPEG4 compression ratio) = 14,400 Mb/s
For the newer cameras: 6 cameras x 1080p x 25 fps x 100 (H.264 compression ratio) = 162,000 Mb/s
Total approximate throughput requirement: 176,400 Mb/s
Task 4: Learning reflection
In this week's tutorial activities, I have learned about several network technologies, including ARP tables and ping packet captures. I have also designed a small network for a friend who purchased security cameras. Completing this task required me to draw a network diagram, list equipment to be purchased, and calculate approximate throughput requirements. In addition, I have used different types of tools including PowerShell, Wireshark, ping, and GetNet-Adapoter that helped me learn how to use different networking devices to gather information. Overall, this week's activities provided us with valuable insights into networking technologies and their practical applications.
