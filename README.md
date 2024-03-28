<h1>Port Security</h1>

<h2>Description</h2>
This lab will configure Switch Port Security.<br/>
<br/>

Switch port security is a feature implemented on network switches to enhance security by controlling access to individual switch ports based on the MAC (Media Access Control) addresses of devices connected to them. The primary goal of switch port security is to prevent unauthorized devices from gaining network access through physical ports on the switch.<br/><br/>

Port Security can be configured as Static, Dynamic, Sticky-Mac, or Maximum.
Port Secuirty can be configured with the violation options Shutdwon, Protect, or Restrict.

<h2>Environments Used </h2>

- <b>Packet Tracer</b>

<h2>Lab walk-through:</h2>

<p align="center">
<h4>Lab Topology:</h4>
<img src="https://i.imgur.com/RFzM6Si.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

<h4>Static configuartion with a Shutdown Violation:</h4> 
In Static configuraion the administrator will manually configure the MAC addresses of devices allowed to access a particular switch port .<br/>
In the Shutdown violation, the interface is placed into error-diabled state, blocking all traffic.<br/>
This configuration is will affect PC1
<img src="https://i.imgur.com/GqcCNLZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/><br/>
The switch has learnt the MAC address and the Violation parametre.
<img src="https://i.imgur.com/Xs7eZPt.png" height="80%" width="80%" alt="Disk Sanitization Steps"/><br/>
<br />

<h4>Dynamic configuarion with a Restrict Violation:</h4> 
In Dynamic configuraion the switch will dynamically learn the MAC addresses of devices allowed to access a particular switch port .<br/>
In the Restrict Violation, traffic from unauthorised addresses is dropped, logged and the violation counter is incremented. Traffic from allowed addresses in forwaded.<br/>
This configuration will affect  PC2
<img src="https://i.imgur.com/50XLs5S.png" height="80%" width="80%" alt="Disk Sanitization Steps"/><br/>
The switch has learnt the MAC address and the Violation parametre.
<img src="https://i.imgur.com/AmWNP3E.png" height="80%" width="80%" alt="Disk Sanitization Steps"/><br/>
<br />

<h4>Sticky configuarion with a Protect Violation:</h4> 
Sticky port security is a feature available on some network switches that combines elements of both static and dynamic port security. The switch will dynamically learn the MAC addresses of device allowed to access a particular switch and it will add it to the running configuration port<br/>
In the Protect Violation, traffic from unauthourised addresses is dropped. Traffic from allowed addresses is forarded.<br/>
This configuration will affect PC3
<img src="https://i.imgur.com/csw2PrB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/><br/>
The switch has learnt the MAC address and the Violation parametre.
<img src="https://i.imgur.com/jbCJgAa.png" height="80%" width="80%" alt="Disk Sanitization Steps"/><br/>
<br />

<h4>Maximum configuarion with a Shutdown Violation:</h4> 
In Maximum configuraion the switch will dynamically learn the MAC addresses of devices allowed to access a particular switch por, upto a specified maximum number.<br/>
In the Shutdown violation, the interface is placed into error-diabled state, blocking all traffic.<br/>
This configuration will affect SWITCH 2 and PC's 4.5 and 6
<img src="https://i.imgur.com/IWCwuii.png" height="80%" width="80%" alt="Disk Sanitization Steps"/><br/>
The switch has learnt the MAC address and the Violation parametre.
<img src="https://i.imgur.com/Vo3yG5m.png" height="80%" width="80%" alt="Disk Sanitization Steps"/><br/>
<br />
