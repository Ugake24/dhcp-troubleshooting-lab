<h1>DHCP troubleshooting</h1>

<h2>Description</h2>
This project focuses on identifying why a client is not receiving an IP address from the DHCP server.
<br />
<br />




<h2>Environments Used </h2>

- <b>Windows server 2025</b>
- <b>Windows 11</b>
<br />

Step1-First, on the client’s computer, we begin troubleshooting by using the command "ipconfig /all" and observe that the IP address is an APIPA address.<br/><br/>
<img src="https://i.imgur.com/LQLeqoG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Step2-Then, we check the client’s services and confirm that everything is working correctly on the client side, indicating that the issue is more general.
<br/><br/>
<img src="https://i.imgur.com/670V8eo.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Step3-Then, we go to the server side and check the services to verify if the DHCP service is running. We notice that it is down.
We activate the service, and it is running again.
<br/>
<br/><br/>
<img src="https://i.imgur.com/YSlLkxC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Step4-Finally, we use the command "ipconfig /renew" to obtain a new IP address from the DHCP server, and everything works properly.<br/><br/>
<img src="https://i.imgur.com/FTcTHpH.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<h2>Conclusion</h2>
This lab demonstrates a real-world troubleshooting scenario involving DHCP failure. By systematically identifying the issue, verifying configurations, and restoring the DHCP service, network connectivity was successfully re-established.


<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
