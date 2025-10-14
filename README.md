<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 (22H2)
- Ubuntu Server 22.04

<h2>High-Level Steps</h2>

- Create a resource group, virtual network, and deploy both Windows and Ubuntu virtual machines in Azure.
- Configure inbound security rules on the Network Security Groups (NSGs) to deny RDP, SSH, HTTP, and ICMP traffic between the VMs.
- Connect to the Windows VM via Remote Desktop, install and open Wireshark, and observe the network traffic between the Windows and Ubuntu VMs using various protocols.
- Observe and analyze the captured network traffic in Wireshark, then modify NSG rules to see how traffic behavior changes when rules are added, removed, or restricted.

<h2>Actions and Observations</h2>

<p>
<img width="2559" height="1391" alt="image" src="https://github.com/user-attachments/assets/f523d689-5966-4556-a05f-a1ef55658c8f" />

</p>
<p>
In the network settings of the Ubuntu VM, we add inbound security rules to the Network Security Groups to deny ping, which we established to observe the results in Wireshark on the Windows VM.
</p>
<br />

<p>
<img width="2560" height="1440" alt="image" src="https://github.com/user-attachments/assets/c842097c-1d3a-4bd4-b1c7-dfe1e555652d" />


</p>
<p>
We see the results of the inbound security rules taking effect; it has put a timeout on the continuous ping we established by PowerShell.
</p>
<br />

<p>
<img width="2560" height="1440" alt="image" src="https://github.com/user-attachments/assets/75d2bad5-d8c1-4434-a985-edd224fbe8da" />

</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
