<h1>DHCP troubleshooting</h1>

<h2>Description</h2>
This project focuses on identifying why a client is not receiving an IP address from the DHCP server.
<br />
<br />




<h2>Environments Used </h2>

- <b>Windows server 2025</b>
- <b>Windows 11</b>
<br />

First, on the client’s computer, we begin troubleshooting by using the command "ipconfig /all" and observe that the IP address is an APIPA address.<br/><br/>
<img src="https://i.imgur.com/LQLeqoG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Then, we check the client’s services and confirm that everything is working correctly on the client side, indicating that the issue is more general.
<br/><br/>
<img src="https://i.imgur.com/670V8eo.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Reducing lease time allows faster reassignment during testing.<br/>
<img src="https://i.imgur.com/nzZR8r0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Configured a DHCP scope to dynamically assign IP addresses<br/>
<img src="https://i.imgur.com/mwFT6DY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />



<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
