# azure-network-protocols
<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this walkthrough, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />




<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 (22H2)
- Ubuntu Server 20.04

<h2>High-Level Steps</h2>

- Step 1: Create resource groups and storage in Microsoft Azure
- Step 2  Create Azure virtual networks and subnets
- Step 3: Create Azure virtual machines for Windows 10 and Linux Ubuntu
- Step 4: Create Azure network security groups
- Step 5: Utilize Microsoft Remote Desktop to connect to connect 2 virtual machines
- Step 6: Install Wireshark to inspect traffic between Azure virtual machines

<h2>Actions and Observations</h2>

<p>   
</p>
1.) Create a Resource Group in Microsoft Azure. 
<img src="https://i.imgur.com/4If8Vds.png" height="50%" width="50%" alt="OS Ticket Resource Group Creation"/>
</p>

Create a Storage Account in Microsoft Azure.
</p>
<img src="https://i.imgur.com/o9HJA3f.png" height="50%" width="50%" alt="OS Ticket Storage Account Creation"/>
</p>
2.) Create a virtual machine in Microsoft Azure with Windows 10, a Virtual Network, and Subnet.
</p>
<img src="https://i.imgur.com/CtOLJuo.png" height="50%" width="50%" alt="OS Ticket VM Creation"/>

</p>
3.) Create virtual machine in Microsoft Azure with Linux (Ubuntu) and deploy.
</p>
<img src="https://i.imgur.com/SzLnmiV.png" height="50%" width="50%" alt="Virtual Machine Linux"/>
</p>

Utilize Microsoft Remote Desktop to access Windows 10 virtual machine
<p>
<img src="https://i.imgur.com/q4R7hqD.png" height="50%" width="50%" alt="Remote Desktop"/>
</p>
Utilize Wireshark to capture packets using Interet Control Messaging Protocol (ICMP) 
</p>
<img src="https://i.imgur.com/yMWgiST.png" height="50%" width="50%" alt="Wireshark"/>
</p>
<br />
<img src="https://i.imgur.com/fRlTG2w.png" height="50%" width="50%" alt="Wireshark"/>
</p>

Utilize Wireshark to capture packets using Secure Shell (SSH)
</p>
<br />
<img src="https://i.imgur.com/ivDUljU.png" height="50%" width="50%" alt="Wireshark"/>
</p>

Utilize Wireshark to monitor DHCP traffic over the network after renewing IP address
</p>
<br />
<img src="https://i.imgur.com/A3b81O6.png" height="50%" width="50%" alt="Wireshark"/>
</p>

Utilize Wireshark to monitor DNS traffic over the network use nslookup to determine "Google" IP addresses
</p>
<br />
<img src="https://i.imgur.com/xd9SCFY.png" height="50%" width="50%" alt="Wireshark"/>
</p>

Utilize Wireshark to monitor ICMP traffic over the network use Ping -t.  
</p>
<br />

<img src="https://i.imgur.com/L6fWZTN.png" height="50%" width="50%" alt="Wireshark"/>
</p>
Create firewall rule to deny inbound ICMP traffic
