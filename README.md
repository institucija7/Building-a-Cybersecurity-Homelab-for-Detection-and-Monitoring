<h1>Creating Vulnerability Management Lab</h1>

<h2>Description</h2>

- <h1>🔭Project consist of:</h1>

- [Downloading the configuration Nessus Vulnerability Scanner](https://www.tenable.com/products/nessus/nessus-essentials)
- [Downloading Virtual Box](https://www.virtualbox.org/wiki/Downloads)
- [Set up Windows10 inside of Virtual Box](https://www.microsoft.com/en-us/software-download/windows10)
- [Install old depricated software on Windows10 VM](https://ftp.mozilla.org/pub/firefox/releases/3.6.12/win32/en-US/)
- <b>[Vulnerability scans agains Windows10 VM using credentials]</b>
- <b>[Remediate and patching Windows10 VM]</b>
 


<h2>Environments Used </h2>

- <b>Windows 10 and Web App Nessus Vuln Scanner</b> 

<h2>Program walk-through:</h2>

<p align="center">
Launch Windows 10VM, set Network to Bridged: <br/>
<img src="https://i.imgur.com/KYC6Aty.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Turn off Windows defender on Windows10VM:  <br/>
<img src="https://i.imgur.com/latFshj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Go to Services and Enable Remote Registries, so our scanner can connect through Registry: <br/>
<img src="https://i.imgur.com/nCIbXbg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Confirm your selection:  <br/>
<img src="https://i.imgur.com/cdFHBiU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Wait for process to complete (may take some time):  <br/>
<img src="https://i.imgur.com/JL945Ga.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Sanitization complete:  <br/>
<img src="https://i.imgur.com/K71yaM2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
