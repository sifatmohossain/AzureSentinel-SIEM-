# <h1>Active Directory Home Lab</h1>


<h2>Description</h2>
This repository contains steps on how I set up a basic home lab running the Active Directory 
<br />


<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b> 
- <b>Oracle VirtualBox</b>

<h2>Environments Used </h2>

- <b>Windows 10 ISO</b> 
- <b>Windows Server 2019 ISO</b>

<h2>Lab walk-through:</h2>

<p align="Center">
Diagram of the Lab: <br/>
<img src="https://i.imgur.com/RLMHsXF.png" height="60%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
Create a new virtual machine by clicking on "New" in VirtualBox, naming it "Domain Controller," and selecting the "Windows Server 2019" ISO file as the boot media. <br/>
<img src="https://i.imgur.com/EtUFiSS.png" height="60%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
Configure the virtual machine by giving it two network adapters: one for connecting to the internet and the other for the private network. <br/>
<img src="https://i.imgur.com/gBlXDdI.png" height="60%" width="50%" alt="Disk Sanitization Steps"/>
<br />
  <br/>
<img src="https://i.imgur.com/2C4fjAd.png" height="60%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
Install Server 2019 on the virtual machine and assign an IP address for the internal network. <br/>
<img src="https://i.imgur.com/ke3NC8M.png" height="60%" width="50%" alt="Disk Sanitization Steps"/>
<br />
  <br/>
<img src="https://i.imgur.com/jkURjaK.png" height="60%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
Name the server and install Active Directory to create the domain. <br/>
<img src="https://i.imgur.com/9X17sgJ.png" height="60%" width="50%" alt="Disk Sanitization Steps"/>
<br />
  <br/>
<img src="https://i.imgur.com/MJjoBaj.png" height="60%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
Configure routing so that clients on the private network can access the internet through the domain controller. <br/>
<img src="https://i.imgur.com/0dXq6q4.png" height="60%" width="50%" alt="Disk Sanitization Steps"/>
<br />
  <br/>
<img src="https://i.imgur.com/bo7wEed.png" height="60%" width="50%" alt="Disk Sanitization Steps"/>
<br />
  <br/>
<img src="https://i.imgur.com/4ZmjdlT.png" height="60%" width="50%" alt="Disk Sanitization Steps"/>
<br />
  <br />
Set up DHCP on the domain controller.<br/>
<img src="https://i.imgur.com/DEjwNO7.png" height="60%" width="50%" alt="Disk Sanitization Steps"/>
<br />
  <br/>
<img src="https://i.imgur.com/5J8RZQD.png" height="60%" width="50%" alt="Disk Sanitization Steps"/>
<br />
    <br />
Run the PowerShell script to create 1000 users in Active Directory. Then, create a new virtual machine named "Client1" and install Windows 10 on it. After creating the new VM, connect the client machine to the private network and join it to the domain.<br/>
<img src="https://i.imgur.com/csnehjs.png" height="60%" width="50%" alt="Disk Sanitization Steps"/>
<br />
  <br/>
<img src="https://i.imgur.com/DSSfFdK.png" height="60%" width="50%" alt="Disk Sanitization Steps"/>
<br />
  <br/>
<img src="https://i.imgur.com/qaFyOQ4.png" height="60%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
Log into the client machine with a domain account. <br/>
<img src="https://i.imgur.com/Q6hJDgM.png" height="60%" width="50%" alt="Disk Sanitization Steps"/>
</p>

