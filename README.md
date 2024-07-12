<h1>Web Application Security Practice with OWASP ZAP on OWASP Juice Shop and Damn Vulnerable Web Application (DMVWA)</h1>



<h2>Description</h2>
This repository contains my practice work on web application security, focusing on testing, scanning and Brute-Forcing using OWASP ZAP. I used OWASP Juice Shop and DMVWA as the sample web application to explore various security vulnerabilities and testing methodologies.
<br />


<h2>Utilities Used</h2>

- <b>OWASP ZAP</b> 
- <b>OWASP JUICE</b>
- <b>Damn Vulnerable Web Application (DMVWA)</b>

<h2>Environments Used </h2>

- <b>Kali Linux</b> 

<h2>Program walk-through:</h2>

<h2>Automated Scan</h2>

Launched ZAP:  <br/>
<img src="https://i.imgur.com/yO0ikLJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
OWASP Juice Shop:  <br/>
<img src="https://i.imgur.com/EcWnQDZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Scan Result:  <br/>
<img src="https://i.imgur.com/VfJ7Mp2.jpeg" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Challenge Resolved: <br/>
<img src="https://i.imgur.com/lXNnThm.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Damn Vulnerable Web Application (DMVWA):  <br/>
<img src="https://i.imgur.com/WrstKNM.png" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/tTn3NS7.png" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

<h2>Manual Scan</h2>

<p align="center">
Performing Manual Scan: <br/>
<img src="https://i.imgur.com/6OJzuxR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/Qr671Gb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Go to Local Server/Proxies and set the browser proxy settings in address and port: <br/>
<img src="https://i.imgur.com/EKnb98L.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Modify Proxy Properties: <br/>
<img src="https://i.imgur.com/YhcInbO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Navigate to Server Certificates and save the certificate somewhere you'll remember and not delete in your files: <br/>
<img src="https://i.imgur.com/SBFyo1A.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/vhNA0qY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Open Firefox, navigate to your preference and search for certificates. Click "View Certificates", then "Import" and navigate to the earlier downloaded certificate. Open it and Trust the Certificate to Websites and Emails: <br/>
<img src="https://i.imgur.com/fK4mbyW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/CLOrxty.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Navigate to "Proxy Settings" to configure your Firefox Proxy settings: <br/>
<img src="https://i.imgur.com/5t9jdlG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/IRWx2Fk.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Login to DMVWA: <br/>
<img src="https://i.imgur.com/VFehRhH.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/WEet6lj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Once logged in, navigate to DMVWA security tab and set the security level to low: <br/>
<img src="https://i.imgur.com/ysGCPCx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Configured Authenticated token, to use the tool to scan authenticated web pages: <br/>
<img src="https://i.imgur.com/y6zY6zc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Re scanned the application. (Notice it picked up more Vulnerabilities because it's able to see all of the sectors of DMVWA that was previously behind the login page): <br/>
<img src="https://i.imgur.com/i0Cn9qC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/IZ9kz3e.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

<h2>Brute-Force Web Login</h2>

<img src="https://i.imgur.com/KsPUco9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Navigate to the "Get" request and open the "Fuzz" menu: <br/>
<img src="https://i.imgur.com/IbgR847.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/LaCbtas.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Then highlight the password attempted and add a wordlist. Then select the area of the request you wish to replace with other data: <br/>
<img src="https://i.imgur.com/n6RGtyM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
After running the "Fuzzer", sort the state tab to show Reflected results first: <br/>
<img src="https://i.imgur.com/VErSF5K.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Brute-Force Successful: <br/>
<img src="https://i.imgur.com/wyf7M9y.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

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
