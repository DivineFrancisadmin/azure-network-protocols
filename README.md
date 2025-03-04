<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04

<h2>High-Level Steps</h2>

- Create Virtual Machines and Network Setup
- Monitor Network Traffic with Wireshark
- Configure and Test Firewall Rules (NSG)
- Analyze Different Network Protocols in Wireshark

<h2>Actions and Observations</h2>

<p>
Create Virtual Machines and Network Setup
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To begin the lab, I first create a Resource Group in the Azure Portal to organize all related resources. Next, I deploy a Windows 10 Virtual Machine (VM), ensuring that it creates a new Virtual Network (VNet) and Subnet for communication. Once the Windows VM is set up, I proceed to create a Linux (Ubuntu) VM, making sure that it is in the same Resource Group and Virtual Network as the Windows VM. This setup ensures both machines can communicate internally without requiring external internet access.</p>
<br />

<p>
  Monitor Network Traffic with Wireshark
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Once my virtual machines are running, I use Remote Desktop to connect to the Windows 10 VM. The first step is to install Wireshark, a network protocol analyzer, which will allow me to inspect network traffic in real time. After installation, I start a packet capture in Wireshark and filter for ICMP traffic. To generate ICMP traffic, I retrieve the private IP address of the Ubuntu VM and attempt to ping it from the Windows 10 VM. I observe the ping requests and replies appearing in Wireshark. Additionally, I open PowerShell or Command Prompt and attempt to ping a public website (e.g., www.google.com) to analyze outbound ICMP traffic.</p>
<br />

<p>
  Configure and Test Firewall Rules (NSG)
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
