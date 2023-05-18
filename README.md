# Setup a Watchguard Firewall
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
<br/> 
•	Admin , readwrite are the default login credentials
<br/>
<br/>
•	Create new Configuration, next -> Confirm your firebox is online, choose “Keep the default DHCP external interface settings” and click next <br/>
•	Choose Domain name and assign DNS server as 9.9.9.9 
<br/>
<br/> 
<img src="https://i.imgur.com/fcbErhC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/ 
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
•	Once on firewall, Got to Network -> interfaces, Set one of the interfaces to Switchout, mark as VLAN 
<br/>
<img src="https://i.imgur.com/7xVxCF1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/ <br/>
<br/>
<br/>
<img src="https://i.imgur.com/WifCnNa.png" height="80%" width="80%" alt="Disk Sanitization Steps"/ 
<br/> 
<br/>
<br/>
<br/>
•	Then go to VLANs <br/>
•	Mark each VLAN to tagged traffic (BUT NOT YOUR MGMT VLAN, this will be untagged) <br/>
<br/> 
<img src="https://i.imgur.com/NeN7xMG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/
<br/>
<br/>
<br/>
<br/>
•	Go to network tab and choose domain, starting/ending IP, and DNS servers  <br/>
<img src="https://i.imgur.com/gDByGfn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/
<br/>
<br/>
<br/>
<br/> 
• Rinse and repeat until VLANs are created <br/> 
<br/>
<img src="https://i.imgur.com/IC9BYdB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/ 
<br/>
<br/>
<br/> 
•	Go to Authentication tab, servers- Find Firebox-DB. Add self as user <br/>
<br/> 
<img src="https://i.imgur.com/qYJx1Vn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/
<br/>
<br/>
<img src="https://i.imgur.com/NFo5hX3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/
<br/>
<br/>
<br/>
<br/>
•	Our Firewall is now completely setup! <br/>
