Your network manager is impressed with your performance in your job as a LAN technician. he would like you to demonstrate your ability to Confirm that all devices are properly configured and troubleshoot any issue. 
Your tasks include verify all network devices have the basic configurations. configure a DHCP server to provide IP address dynamically, setting our own DNS server for our Web server

In this activity you will configure the YT-R-01 router, YT-SW-01 switch, DHCP, DNS, Web Server

## Packet Tracer Project - Network Configuration

### 1. DNS Server A Records
<p align="center">
  <img src="images/01.png" alt="DNS A records for breadcrumb domains" width="80%">
  <br><strong>DNS A records pointing multiple www.breadcrumb.* domains to 192.168.10.5</strong>
</p>

### 2. Web Server (YT-WEB) Services & Files
<p align="center">
  <img src="images/02.png" alt="Web server HTTP/HTTPS and HTML files" width="80%">
  <br><strong>HTTP and HTTPS enabled; hosted files: index.html, helloworld.html, image.html, copyrights.html</strong>
</p>

### 3. Switch CLI Configuration (YT-SW-01)
<p align="center">
  <img src="images/03.png" alt="Switch basic config" width="80%">
  <br><strong>Hostname, passwords, VLAN 1 IP 192.168.10.2/24, write memory</strong>
</p>

### 4. DHCP Server Pool Settings
<p align="center">
  <img src="images/04.png" alt="DHCP pool configuration" width="80%">
  <br><strong>Pool: serverPool • Start: 192.168.10.10 • Mask: /24 • Gateway: 192.168.10.1 • DNS: 192.168.10.3</strong>
</p>

### 5. DNS Server IP Configuration
<p align="center">
  <img src="images/05.png" alt="DNS server static IP" width="80%">
  <br><strong>Static IPv4: 192.168.10.3/24 • Gateway: 192.168.10.1 • DNS: self</strong>
</p>

### 6. DHCP Client Assignment (Server)
<p align="center">
  <img src="images/06.png" alt="DHCP client received IP" width="80%">
  <br><strong>DHCP server interface received 192.168.10.4 via DHCP</strong>
</p>

### 7. Router CLI Configuration (YT-R-01)
<p align="center">
  <img src="images/07.png" alt="Router basic config" width="80%">
  <br><strong>Hostname, passwords, G0/0: 192.168.10.1/24, no shutdown</strong>
</p>

### 8. Web Server IP (YT-WEB)
<p align="center">
  <img src="images/08.png" alt="Web server DHCP IP" width="80%">
  <br><strong>YT-WEB received 192.168.10.5 via DHCP</strong>
</p>

### 9. Simulation - DHCP Packet Flow
<p align="center">
  <img src="images/09.png" alt="DHCP packet exchange" width="80%">
  <br><strong>DHCP Discover/Offer/Request/Ack captured in simulation</strong>
</p>

### 10. Overall Logical Topology
<p align="center">
  <img src="images/10.png" alt="Full network topology" width="80%">
  <br><strong>Complete logical view: router, switch, servers, client PCs</strong>
</p>
