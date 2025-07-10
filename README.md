<h1>Active Directory Home Lab</h1>


<h2>Overview</h2>
This project demonstrates a functional Windows Server 2019 Active Directory lab built using VirtualBox. It simulates a basic enterprise network with a domain controller, DHCP, NAT, and a domain-joined Windows 10 client. A PowerShell script was used to create 1000 users for testing administrative tasks.

<br />

<h2>Objective</h2>
Learn how organizations manage users, computers, and network settings through Active Directory.

<h2>Tools Used</h2>

- <b>VirtualBox</b> 
- <b>Windows Server 2019</b>
- <b>Windows 10</b>
- <b>Active Directory Domain Services (AD DS)</b>
- <b>DHCP</b>
- <b>Routing and Remote Access (NAT)</b>
- <b>PowerShell</b>

<h2>Key Features</h2>

- <b>Configured DC with two NICs (NAT + Internal)</b> 
- <b>Promoted Server 2019 to Domain Controller with root domain</b>
- <b>Installed and configured DHCP for internal network</b>
- <b>Configured NAT using Routing and Remote Access</b>
- <b>Created 1000 domain users using PowerShell</b>
- <b>Created organizational units and assigned domain admin</b>
- <b>Joined Windows 10 client to the domain</b>
- <b>Tested login with domain account on client VM</b>


<h2>Project walk-through:</h2>
<br/>

<p align="center">
DC VM configured with two NICs: NAT for internet access, Internal Network for local domain communication: 
<br/>
 
<br/>
<img src="https://i.imgur.com/DlKlKgh.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>
<br />
 
<br/>
<img src="https://imgur.com/RCQtWUN.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>
<br />

 
<br/>

 
<br />
Static IP assigned to internal NIC. This ensures the domain controller can reliably handle DNS and DHCP for the internal network:  
<br/>

<br/>
<img src="https://i.imgur.com/sWXeEsx.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>
<br />

<br/>

<br />
AD DS installed on Server 2019 to enable domain controller promotion: 
<br/>

<br/>
<img src="https://i.imgur.com/csFra62.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>
<br />

<br/>

<br />
Promoting the server to a domain controller and creating a new root domain:  
<br/>

<br/>
<img src="https://i.imgur.com/K3kTPgq.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>
<br />

<br/>

<br />
Successfully promoted to domain controller. Logged in as domain administrator:  
<br/>

<br/>
<img src="https://i.imgur.com/JL945Ga.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>
<br />

<br/>

<br />
Created organizational unit to manage admin users separately from standard accounts:  
<br/>

<br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>
<br />

<br/>

<br />
Domain admin account manually created and assigned proper privileges:  
<br/>

<br/>
<img src="https://i.imgur.com/JL945Ga.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>
<br />

<br/>

<br />
Configured DHCP to automatically assign IP addresses to internal network clients:  
<br/>

<br/>
<img src="https://i.imgur.com/JL945Ga.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>
<br />

<br/>

<br />
Windows 10 client successfully obtained IP from DHCP scope via internal network:  
<br/>

<br/>
<img src="https://i.imgur.com/JL945Ga.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>
<br />

<br/>

<br />
NAT enabled on the DC to allow the internal network to access the internet through the external NIC:  
<br/>

<br/>
<img src="https://i.imgur.com/JL945Ga.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>
<br />

<br/>

<br />
Used PowerShell to automate creation of 1000 Active Directory users for simulation and testing:  
<br/>

<br/>
<img src="https://i.imgur.com/JL945Ga.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>
<br />

<br/>

<br />
Users successfully imported into Active Directory using the script:  
<br/>

<br/>
<img src="https://i.imgur.com/JL945Ga.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>
<br />

<br/>

<br />
Windows 10 client VM configured to communicate on internal network with domain controller:  
<br/>

<br/>
<img src="https://i.imgur.com/JL945Ga.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>
<br />

<br/>

<br />
Successfully joined the client VM to the domain created on the DC:  
<br/>

<br/>
<img src="https://i.imgur.com/JL945Ga.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>
<br />

<br/>

<br />
Demonstrating successful domain login from a client device using Active Directory credentials:  
<br/>

<br/>
<img src="https://i.imgur.com/JL945Ga.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>
<br />

<br/>

<br />
Internet access verified from client VM via domain controller’s NAT routing:  
<br/>

<br/>
<img src="https://i.imgur.com/JL945Ga.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>
</p>


<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
