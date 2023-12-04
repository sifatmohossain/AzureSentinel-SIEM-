# <h1>Azure Sentinel (SIEM)</h1>


<h2>Description</h2>
In this project, I setup Azure Sentinel (SIEM) and connect it to a live virtual machine acting as a honey pot. I observed live attacks (RDP Brute Force) from all around the world. I used a custom PowerShell script to look up the attackers Geolocation information and plot it on the Azure Sentinel Map. 
<br />


<h2>Languages and Utilities Used</h2>

- <b>PowerShell Script</b> 
- <b>Azure Sentinel</b>
- <b>Kusto Query Language (KQL - Used to build world map)</b>
- <b>3rd Party API: ipgeolocation.io</b>


<h2>Project walk-through:</h2>

<p align="Center">
Diagram of the project: <br/>
<img src="https://i.imgur.com/e63D0r4.png" height="60%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
 Create a Honeypot Virtual Machine<br/>
<img src="https://i.imgur.com/fI00p8J.png" height="60%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<img src="https://i.imgur.com/4Lw0EHJ.png" height="60%" width="50%" alt="Disk Sanitization Steps"/>
<br />
  <br/>
<img src="https://i.imgur.com/qij8Pux.png" height="60%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
 Create a Log Analytics Workspace <br/>
<img src="https://i.imgur.com/cedltBx.png" height="60%" width="50%" alt="Disk Sanitization Steps"/>
<br />
  <br />
 Configure Microsoft Defender for Cloud <br/>
<img src="https://i.imgur.com/M2boD0x.png" height="60%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
Name the server and install Active Directory to create the domain. <br/>
<img src="https://i.imgur.com/JmpKPvt.png" height="60%" width="50%" alt="Disk Sanitization Steps"/>
<br />
  <br />
 Connect Log Analytics Workspace to Virtual Machine <br/>
<img src="https://i.imgur.com/zt2JBUZ.png" height="60%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
Configure Microsoft Sentinel <br/>
<img src="https://i.imgur.com/MNquzye.png" height="60%" width="50%" alt="Disk Sanitization Steps"/>
<br />
  <br />
 Disable the Firewall in Virtual Machine <br/>
<img src="https://i.imgur.com/CXygZCO.png" height="60%" width="50%" alt="Disk Sanitization Steps"/>
<br />
  <br />
 Scripting the Security Log Exporter <br/>
<img src="https://i.imgur.com/KZtCfSz.png" height="60%" width="50%" alt="Disk Sanitization Steps"/>
<br />
  <br />
Set up your account on ipgeolocation.io.<br/>
<img src="https://i.imgur.com/BHxlscn.png" height="60%" width="50%" alt="Disk Sanitization Steps"/>
<br />
  <br />
  Create Custom Log in Log Analytics Workspace
  <br/>
<img src="https://i.imgur.com/C86AYAj.png" height="60%" width="50%" alt="Disk Sanitization Steps"/>
<br />
    <br />
Query the Custom Log.<br/>
<img src="https://i.imgur.com/5OwEfar.png" height="60%" width="50%" alt="Disk Sanitization Steps"/>
<br />
  <br />
 Extract Fields from Custom Log <br/>
<img src="https://i.imgur.com/S5H04mn.png" height="60%" width="50%" alt="Disk Sanitization Steps"/>
<br />
  <br />
 Map Data in Microsoft Sentinel <br/>
<img src="https://i.imgur.com/5C1dSOh.png" height="60%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<img src="https://i.imgur.com/HEok3af.png" height="60%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<img src="https://i.imgur.com/EL2EYlL.png" height="60%" width="50%" alt="Disk Sanitization Steps"/>
</p>

