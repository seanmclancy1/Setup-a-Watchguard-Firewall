# Setup-a-Watchguard-Firewall
Firebox T20 Walkthrough | Watchguard
<h2>Description</h2>
 Our company uses Watchguard Firewall products when we build networks for clients (when possible). Watchguard Firewall provides a cost-effective, powerful interface that is able to mangage and monitor network traffic while maintaning security. We will be doing a basic walkthrough on how to setup a Firebox T20.
<br />

<h2>Program walk-through:</h2>

<p align="center">
<br/>
•	Before starting this guide you can reference the following links for the quick start guide as well as the hardware guide.
<br/>
https://www.watchguard.com/help/docs/help-center/en-US/Content/en-US/Fireware/installation/qsg_firebox.html 
<br/>
https://www.watchguard.com/help/docs/help-center/en-US/Content/en-US/Hardware-Guides/firebox-t20-hardware-guide.html
<br/>
<img src="https://i.imgur.com/yjB21Ue.png" height="80%" width="80%" alt="Disk Sanitization Steps"/
<br/>
<br/>
<br/>
<br/>
•	Today we will be setting up a Firebox T20.
<br/>
<br/>
<img src="https://i.imgur.com/nXEblrG.jpg" width="80%" alt="Disk Sanitization Steps"/
<br/>
<br/>
<br/>
<br/>
•	The first thing we need to do is setup and register a new account, then sign in.
<br/>
https://accountmanager.cloud.watchguard.com/create-account
<br/>
<img src="https://i.imgur.com/XSC7GSt.png" height="80%" width="80%" alt="Disk Sanitization Steps"/
<br/>
<br/>
<br/>
• The firebox will come with a small pamphlet detailing the activation steps. <br/>
<br/>
<img src="https://i.imgur.com/UwvvXRq.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/
<br/>
<br/>  
•	Activate Firebox (watchguard.com/activate)   
<br/>
<br/>
<img src="https://i.imgur.com/gyV67SX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/
<br/>
<br/>
•	Name your Firebox 
<br/>
<br/>
<img src="https://i.imgur.com/lN4naNP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/
<br/>
<br/>
•	Choose and confirm region <br/>
•	Log into firebox (Default 10.0.1.1:8080) 
<br/>
<br/>
<img src="https://i.imgur.com/LzUbYUj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/
<br/>
•	Admin , readwrite are the default login credentials
<br/>
<br/>
•	Create new Configuration, next -> Confirm your firebox is online, choose “Keep the default DHCP external interface settings” and click next <br/>
•	Choose Domain name and assign DNS server as 9.9.9.9 
<br/>
<br/>  
•	Assign IP range 
<br/>
<br/>  
<img src="https://i.imgur.com/DcJ2gBL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/
<br/>
<br/>
•	Create passphrase to get back into Firebox 
<br/>
<br/>  
<img src="https://i.imgur.com/9p8w9q0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/
<br/>
<br/>
•	Fill in contact information   
<br/>
<br/>  
•	Select time zone   
<br/>
<br/>   
<img src="https://i.imgur.com/IfNCsJi.png" height="80%" width="80%" alt="Disk Sanitization Steps"/
<br/>
<br/>
•	Choose what content you want to filter
<br/>
<br/>
<img src="https://i.imgur.com/hh4T2Ca.png" height="80%" width="80%" alt="Disk Sanitization Steps"/  
<br/>
<br/>
•	Finally look at the overview of what we setup and confirm <br/>
•	Setup has now been completed, Click on “Open Fireware Web UI"   
<br/>
<br/>  
<img src="https://i.imgur.com/8KYQG6x.png" height="80%" width="80%" alt="Disk Sanitization Steps"/  
<br/>
<br/>  
•Connect to UDMP at 192.168.1.1 
<br/>
<img src="https://i.imgur.com/hXaycb6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/ <br/>
<br/>
<br/>
<br/>
• If it tells you to “Enable Config Backup”, go to Settings -> Updates <br/>
<img src="https://i.imgur.com/qvaIR2A.png" height="80%" width="80%" alt="Disk Sanitization Steps"/
<br/>
<br/>
<br/>
<br/>
• Then go to System, click on “Automate Cloud Config Backup” and provide your password to generate the encryption key  <br/>
<img src="https://i.imgur.com/XJbKcnn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/
<br/>
<br/>
•	Now go back and update (Allow UDMP to COMPLETELY update BEFORE plugging in any other devices). 
<br/>
<br/>
<img src="https://i.imgur.com/w5yGv6s.png" height="80%" width="80%" alt="Disk Sanitization Steps"/
<br/>
<br/>
<img src="https://i.imgur.com/Ltn5Ywb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/
<br/>
<br/>
<br/>
<br/>
•	Now go to Settings>Networks> and click on the default router <br/>
<img src="https://i.imgur.com/jltFjwM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br/>
• Change name to MGMT, change address to 10.1.150.1/24 and click Save <br/>
<img src="https://i.imgur.com/oRC8E8c.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br/>
<br/>
• Unplug your computer from UDMP, Reconnect it <br/>
• Verify that your computer is getting a DHCP address in the 10.1.150 scheme (If it is not, your switch and devices will not, so this is very important).
 <br/>
<img src="https://i.imgur.com/3csntTm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br/>
<br/>
<br/>
• Create Remaining Networks as needed.
<br/>
<img src="https://i.imgur.com/vca3Bs7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br/>
<img src="https://i.imgur.com/uuHR10R.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br/>
<br/>
•	It should now look something like this.
<br/>
<img src="https://i.imgur.com/mNcpSKY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br/>
<br/>
<br/>
•We are now going to setup Wifi Networks. Go to Settings -> Wireless Networks. <br/>
• Create Wireless Networks per VLANS above.
<br/>
<img src="https://i.imgur.com/U4cJopR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br/>
<img src="https://i.imgur.com/07GX9cJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br/>
It should now look like this.<br/>
<img src="https://i.imgur.com/yIuRB3d.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br/>
<br/>
<br/>
•	Now we can Pull in Devices <br/>
•	Plug Switches into ports on UDMP.  Ensure they get a DHCP address in the 10.1.150 scheme.  If they don’t, do not adopt them. Figure out why they are not grabbing the proper address (Port profile of their uplink port is a good place to start)—Do not adopt a Unifi device that is not properly on the MGMT LAN. 
<br/>
•	Do not adopt anything else until the switches that are plugged directly into the UDMP are completely updated and adopted.
<br/>
<img src="https://i.imgur.com/f3UEjWS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br/>
• Now we can adopt our Access Points. <br/>
•	REMEMBER- Ports that Switches, Access Points, Etc. are plugged into should have a port profile of ‘All’ and should be pulling an address in the 10.1.150 scheme.  If they are not, stop.  Something is wrong. <br/>
<br/>
<br/>
<br/>
<br/>
• Once all devices are adopted, set static Ips.<br/>
• Go to Network -> Static IP<br/>
•	IP address= Set it to whatever IP is available within that range<br/>
•	Preferred DNS= 9.9.9.9 <br/>
•	Subnet Mask= 255.255.255.0 <br/>
•	Gateway=  10.1.150.1 (the MGMT IP Range) <br/>
<br/>
<img src="https://i.imgur.com/Cayt0cE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br/>
<img src="https://i.imgur.com/8uxKeg0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br/>
<br/>
<br/>
•	For this network I have decided I will also add AC Beacons to quickly extend wireless coverage and improve throughput.
<br/>
<img src="https://i.imgur.com/l4805Aa.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br/>
<br/>
•	Our network is now setup !
<br/>
<img src="https://i.imgur.com/dY0PNhu.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br/>
<img src="https://i.imgur.com/va3EVpl.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
