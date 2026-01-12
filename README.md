Your network manager is impressed with your performance in your job as a LAN technician. he would like you to demonstrate your ability to Confirm that all devices are properly configured and troubleshoot any issue. 
Your tasks include verify all network devices have the basic configurations. configure a DHCP server to provide IP addresses dynamically, setting our own DNS server for our Web server

In this activity, you will configure the YT-R-01 router, YT-SW-01 switch, DHCP, DNS, and Web Server

## Packet Tracer Project - Network Configuration

### 1 - Full Logical Topology Overview
<p align="center">
  <img src="/1.png" alt="Network topology" width="80%">
  <br><strong>Complete layout: router, switch, servers, clients</strong>
</p>

### 2 - DNS Server Physical Modules
<p align="center">
  <img src="/2.png" alt="DNS physical view" width="80%">
  <br><strong>WMP300N wireless module installed</strong>
</p>

### 3 - Router CLI (YT-R-01)
<p align="center">
  <img src="/3.png" alt="Router config" width="80%">
  <br><strong>G0/0: 192.168.10.1/24, passwords, no shutdown</strong>
</p>

### 4 - Switch CLI & Security (YT-SW-01)
<p align="center">
  <img src="/4.png" alt="Switch config" width="80%">
  <br><strong>Hostname, passwords, VLAN1 192.168.10.2/24, enable secret</strong>
</p>

### 5 - Switch CLI (early config stage)
<p align="center">
  <img src="/5.png" alt="Switch early CLI" width="80%">
  <br><strong>YT-SW-01 initial configuration commands, VLAN1 IP setup</strong>
</p>

### 6 - DHCP Pool Configuration
<p align="center">
  <img src="/6.png" alt="DHCP pool" width="80%">
  <br><strong>Start 192.168.10.10, /24, GW 192.168.10.1, DNS 192.168.10.3</strong>
</p>

### 7 - DHCP Server Interface (received IP)
<p align="center">
  <img src="/7.png" alt="DHCP client IP" width="80%">
  <br><strong>FastEthernet0 got 192.168.10.4 via DHCP</strong>
</p>

### 8 - Router Interface & Basic Settings
<p align="center">
  <img src="/8.png" alt="Router interface config" width="80%">
  <br><strong>YT-R-01 G0/0 IP assignment and no shutdown</strong>
</p>

### 9 - DNS Server IP Config
<p align="center">
  <img src="/9.png" alt="DNS IP" width="80%">
  <br><strong>Static 192.168.10.3/24, GW 192.168.10.1, self as DNS</strong>
</p>

### 10 - Web Server IP (YT-WEB)
<p align="center">
  <img src="/10.png" alt="Web server IP" width="80%">
  <br><strong>Received 192.168.10.5 via DHCP</strong>
</p>

### 11 - Web Server Files & Services
<p align="center">
  <img src="/10.1.png" alt="Web server files" width="80%">
  <br><strong>HTTP/HTTPS on, files: index.html, copyrights.html, etc.</strong>
</p>

### 12 - Sale PC - DHCP Assigned
<p align="center">
  <img src="/11.png" alt="Sale PC IP" width="80%">
  <br><strong>FastEthernet0: 192.168.10.5 via DHCP</strong>
</p>

### 13 - Marketing PC - DHCP Assigned
<p align="center">
  <img src="/12.png" alt="Marketing PC IP" width="80%">
  <br><strong>FastEthernet0: 192.168.10.6 via DHCP</strong>
</p>

### 14 - IT PC - DHCP Assigned
<p align="center">
  <img src="/13.png" alt="IT PC IP" width="80%">
  <br><strong>FastEthernet0: 192.168.10.7 via DHCP</strong>
</p>

### 14 - DHCP Packet Simulation
<p align="center">
  <img src="/14.png" alt="DHCP simulation" width="80%">
  <br><strong>DHCP Discover/Offer/Request/Ack flow</strong>
</p>

