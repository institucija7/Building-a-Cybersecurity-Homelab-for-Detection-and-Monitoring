<h1>Creating Vulnerability Management Lab</h1>

<h2>Description</h2>

- <h1>🔭Project consist of:</h1>

- [Downloading the configuration Nessus Vulnerability Scanner](https://www.tenable.com/products/nessus/nessus-essentials)
- [Downloading Virtual Box](https://www.virtualbox.org/wiki/Downloads)
- [Set up Windows10 inside of Virtual Box](https://www.microsoft.com/en-us/software-download/windows10)
- <b>[Remediate and patching Windows10 VM]</b>
 


<h2>Environments Used </h2>

- <b>Windows 10 and Web App Nessus Vuln Scanner</b> 

<h2>Program walk-through:</h2>

<p align="center">
Launch Windows 10VM, set Network to Bridged: <br/>
<img src="https://i.imgur.com/jjTzIHu.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Turn off Windows defender on Windows10VM- Domain,Public and Private:  <br/>
<img src="https://i.imgur.com/atD2YmA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Go to Services and Enable Remote Registries, so our scanner can connect through Registry: <br/>
<img src="https://i.imgur.com/y36OtZO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Enable file and printer sharing:  <br/>
<img src="https://i.imgur.com/dBUGNYB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
User Account Control(make it to lower):  <br/>
<img src="https://i.imgur.com/8fWHIXT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Registry Editor(click on empty field and create DWORD(next picture explained more)):  <br/>
<img src="https://i.imgur.com/EfxNHAq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Create File: LocalAccountTokenFilterPolicy and set Value=1:  <br/>
<img src="https://i.imgur.com/9nidT3Q.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
First scan without Credentials, only 1 Medium vulnerability(for scan take ip from VM- Run command ipconfig in command line and take ip4address): <br/>
<img src="https://i.imgur.com/bO5ygu6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Put Credentials of VM Windows 10: <br/>
<img src="https://i.imgur.com/n7PZvUg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Second Scan with Credentials(a lot Critical and High Vulnerabilities):  <br/>
<img src="https://i.imgur.com/rirn0ZH.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Remediate and patch the VM Windows 10, turn on Firewall:  <br/>
<img src="https://i.imgur.com/zlDMbzF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Go to Nessus scaner, run again scan and if you have some  remediations, scanner will told you exactly what you need to fix <br/>
<img src="https://i.imgur.com/zlDMbzF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>







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
