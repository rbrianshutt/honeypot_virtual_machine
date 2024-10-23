<h1>Setting Up a Honeypot Virtual Machine </h1>

![](https://github.com/rbrianshutt/honeypot_virtual_machine/blob/main/images/honeypot.png)

<h2>Description</h2>
I set up a honeypot virtual machine in Azure.  All firewalls were removed to entice cyber attacks from around the world. I used a custom PowerShell script from to extract metadata to derive the geolocation data.   
<br />

<h2>Techonology used</h2>

- <b>Azure</b> 
- <b>PowerShell ISO</b>
- <b>Custom Powershell script from [Josh Madakor](https://github.com/joshmadakor1/Sentinel-Lab/blob/main/Custom_Security_Log_Exporter.ps1)</b>
- <b>ipgeolocation.io</b>
- <b>Remote Desktop Connection</b>

<h2>Program walk-through:</h2>

<p align="center">
Creating a virtual machine in Azure:  <br/>
 
![](https://github.com/rbrianshutt/honeypot_virtual_machine/blob/main/images/create_virtual_machine.PNG)
<br />
<br />
Setting up the virtual machine:  <br/>

![](https://github.com/rbrianshutt/honeypot_virtual_machine/blob/main/images/setup_virtual_machine.PNG)
<br />
<br />
Disabling firewall protections in VM Windows host to invite cyber attacks:  <br/>

![](https://github.com/rbrianshutt/honeypot_virtual_machine/blob/main/images/disable_fireware.PNG)
<br />
<br />
Custom script in Powershell ISO:  <br/>

![](https://github.com/rbrianshutt/honeypot_virtual_machine/blob/main/images/script_security_log_powershell.PNG)
<br />
<br />
3rd party API using ipgeolation.io.  Get API key and paste in custom Powershell script  Run the Poweshell script :  <br/>

![](https://github.com/rbrianshutt/honeypot_virtual_machine/blob/main/images/ipgeolocation.PNG)
<br />
<br />
Event Viewer showing logon failures indicating brute force attacks:  <br/>

![](https://github.com/rbrianshutt/honeypot_virtual_machine/blob/main/images/event_viewer.PNG)
<br />
<br />
Powershell script is parsing geolocation data from attacks around the world:
<br/>
<br />

![](https://github.com/rbrianshutt/honeypot_virtual_machine/blob/main/images/powershell_script_parsing_data.PNG)
<br />
<br />
Attacks were mostly from Kyiv, Ukraine, but also included locations including Russia, Belize, Netherlands, Turkey, Malaysia, Morocco, Brazil, New York and Washington in the US

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
