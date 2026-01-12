Your network manager is impressed with your performance in your job as a LAN technician. he would like you to demonstrate your ability to Confirm that all devices are properly configured and troubleshoot any issue. 
Your tasks include verify all network devices have the basic configurations. configure a DHCP server to provide IP addresses dynamically, setting our own DNS server for our Web server

In this activity, you will configure the YT-R-01 router, YT-SW-01 switch, DHCP, DNS, and Web Server

## Packet Tracer Project - Network Configuration

## Packet Tracer Project - Network Configuration

### 1. DNS Server A Records
<p align="center">
  <img src="/8.png" alt="DNS A records" width="80%">
  <br><strong>Multiple www.breadcrumb.* A records → 192.168.10.5</strong>
</p>

### 2. Web Server Files & Services
<p align="center">
  <img src="/2.png" alt="Web server files" width="80%">
  <br><strong>HTTP/HTTPS on, files: index.html, copyrights.html, etc.</strong>
</p>

### 3. Switch CLI (YT-SW-01)
<p align="center">
  <img src="/4.png" alt="Switch config" width="80%">
  <br><strong>Hostname, passwords, VLAN1 192.168.10.2/24</strong>
</p>

### 4. DHCP Pool Configuration
<p align="center">
  <img src="/6.png" alt="DHCP pool" width="80%">
  <br><strong>Start 192.168.10.10, /24, GW 192.168.10.1, DNS 192.168.10.3</strong>
</p>

### 5. DNS Server IP Config
<p align="center">
  <img src="/9.png" alt="DNS IP" width="80%">
  <br><strong>Static 192.168.10.3/24, GW 192.168.10.1, self as DNS</strong>
</p>

### 6. DHCP Server Interface (received IP)
<p align="center">
  <img src="/7.png" alt="DHCP client IP" width="80%">
  <br><strong>FastEthernet0 got 192.168.10.4 via DHCP</strong>
</p>

### 7. Switch Security & VLAN Config
<p align="center">
  <img src="/4.png" alt="Switch security" width="80%">
  <br><strong>Passwords (cisco/class), enable secret, no shut VLAN1</strong>
</p>

### 8. Router CLI (YT-R-01)
<p align="center">
  <img src="/3.png" alt="Router config" width="80%">
  <br><strong>G0/0: 192.168.10.1/24, passwords, no shutdown</strong>
</p>

### 9. Web Server IP (YT-WEB)
<p align="center">
  <img src="/10.png" alt="Web server IP" width="80%">
  <br><strong>Received 198.10.5 via DHCP</strong>
</p>

### 10. DHCP Packet Simulation
<p align="center">
  <img src="/10.1.png" alt="DHCP simulation" width="80%">
  <br><strong>DHCP Discover/Offer/Request/Ack flow</strong>
</p>

### 10. DHCP Packet Simulation
<p align="center">
  <img src="/15.png" alt="DHCP simulation" width="80%">
  <br><strong>DHCP Discover/Offer/Request/Ack flow</strong>
</p>

### 11. Sale PC - DHCP Assigned
<p align="center">
  <img src="/11.png" alt="Sale PC IP" width="80%">
  <br><strong>FastEthernet0: 192.168.10.5 via DHCP</strong>
</p>

### 12. Marketing PC - DHCP Assigned
<p align="center">
  <img src="/12.png" alt="Marketing PC IP" width="80%">
  <br><strong>FastEthernet0: 192.168.10.6 via DHCP</strong>
</p>

### 13. DNS Server Physical Modules
<p align="center">
  <img src="/2.png" alt="DNS physical view" width="80%">
  <br><strong>WMP300N wireless module installed</strong>
</p>

### 14. Server Configuration Table
<p align="center">
  <img src="/14.png" alt="Server IP table" width="80%">
  <br><strong>IP summary: router, switch, servers</strong>
</p>

### 15. Full Logical Topology Overview
<p align="center">
  <img src="/1.png" alt="Network topology" width="80%">
  <br><strong>Complete layout: router, switch, servers, clients</strong>
</p>
