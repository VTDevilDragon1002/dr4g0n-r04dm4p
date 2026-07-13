

# IPv4 Addressing

## Definition

**IPv4 (Internet Protocol Version 4)** is the fourth version of the Internet Protocol and the most widely used addressing system. It uses **32-bit addresses**, allowing approximately **4.3 billion unique IP addresses**. Every device connected to a network must have a unique IPv4 address for communication.

IPv4 addresses are written in **dotted-decimal notation**, consisting of four octets separated by periods. Each octet ranges from **0 to 255**. Although IPv4 remains the standard for most networks, the limited number of available addresses has led to the development and adoption of IPv6.

---

# IPv6 Addressing

## Definition

**IPv6 (Internet Protocol Version 6)** is the latest version of the Internet Protocol, developed to overcome the address exhaustion problem of IPv4. It uses **128-bit addresses**, providing an enormous number of unique IP addresses to support the growing number of Internet-connected devices.

IPv6 addresses are written in **hexadecimal notation** and separated by colons. In addition to a larger address space, IPv6 offers simplified routing, automatic address configuration, improved efficiency, and built-in support for modern networking technologies.

---

# Subnetting

## Definition

**Subnetting** is the process of dividing a large network into smaller logical networks called **subnets**. This technique improves network organization, enhances security, reduces broadcast traffic, and allows more efficient utilization of IP addresses.

By separating networks into smaller segments, subnetting makes network management easier, improves overall performance, and isolates network issues or security risks.

---

# CIDR (Classless Inter-Domain Routing)

## Definition

**CIDR (Classless Inter-Domain Routing)** is an IP addressing method that replaces the traditional class-based addressing system. Instead of fixed network classes, CIDR uses variable-length prefixes to allocate IP addresses more efficiently.

CIDR reduces IP address wastage, simplifies routing, minimizes routing table size, and allows Internet Service Providers (ISPs) and organizations to allocate address blocks based on actual requirements.

---

# Routing Basics

## Definition

**Routing** is the process of forwarding data packets from a source network to a destination network through one or more routers. Routers examine destination IP addresses and use routing tables to determine the best available path for packet delivery.

Routing is essential for communication between different networks, including communication across the Internet. It can be performed manually using static routes or automatically using dynamic routing protocols.

## Types of Routing

- Static Routing
- Dynamic Routing
- Default Routing

---

# NAT (Network Address Translation)

## Definition

**Network Address Translation (NAT)** is a networking technique that translates private IP addresses into public IP addresses. It allows multiple devices within a private network to share a single public IP address when accessing the Internet.

NAT conserves public IPv4 addresses, hides internal network addresses from external networks, improves network security, and enables organizations to use private IP addressing while maintaining Internet connectivity.

## Types of NAT

- Static NAT
- Dynamic NAT
- PAT (Port Address Translation)


# 1. Network Architecture

Network Architecture defines how different devices, systems, and protocols are structured and communicate within a network.

---

## 1.1 Network Models

### LAN (Local Area Network)
A LAN is a small network that connects devices within a limited area like a home, office, or lab.

- High speed communication
- Low latency
- Privately managed

Example: Office Wi-Fi network

---

### WAN (Wide Area Network)
A WAN connects multiple LANs across large geographic areas like cities or countries.

- Uses public or leased communication lines
- Higher latency compared to LAN
- Example: Internet

---

### MAN (Metropolitan Area Network)
A MAN covers a city or large campus area.

- Larger than LAN, smaller than WAN
- Example: City-wide ISP network

---

### Hybrid Network
A combination of LAN, MAN, and WAN networks.

- Used in large enterprises
- Flexible and scalable architecture

---

## 1.2 OSI Model

The OSI (Open Systems Interconnection) model defines how data moves through a network in 7 layers.

### Layers:

1. Physical Layer → Cables, signals
2. Data Link Layer → MAC addresses, switching
3. Network Layer → IP addressing, routing
4. Transport Layer → TCP/UDP communication
5. Session Layer → Session management
6. Presentation Layer → Data formatting, encryption
7. Application Layer → User-level applications (HTTP, FTP)

---

## 1.3 TCP/IP Model

A simplified model used in real-world networking.

### Layers:

1. Network Access Layer → Physical + Data Link
2. Internet Layer → IP, routing
3. Transport Layer → TCP/UDP
4. Application Layer → HTTP, DNS, FTP

---

## 1.4 Network Communication Flow

How data moves between two systems:

1. User sends request (Application Layer)
2. Data is broken into packets
3. Packets move through TCP/IP layers
4. Routed across networks using IP
5. Received by destination system
6. Data is reassembled
7. Delivered to application

---


# Network Security

## Entry Level

| Cert | Importance | Notes |
|---|---|---|
| ISC2 Certified in Cybersecurity (CC) | 3 | Free entry-level certification recognized globally |
| CompTIA Network+ (N10-009) | 4 | Industry-standard networking certification |
| Cisco CCNA (200-301 v1.2) | 5 | Most recognized networking certification |
| Fortinet Certified Associate (FCA) | 3 | Covers firewall and network security fundamentals |
| Juniper JNCIA-Junos | 3 | Juniper networking fundamentals |
| Microsoft SC-900 | 3 | Microsoft security, compliance, and identity fundamentals |

---

## Intermediate Level

| Cert | Importance | Notes |
|---|---|---|
| CompTIA Security+ (SY0-701) | 5 | One of the most requested security certifications |
| Cisco CyberOps Associate | 4 | SOC monitoring and incident response |
| Cisco CCNP Security | 4 | Enterprise network security technologies |
| Fortinet Certified Professional (FCP - Network Security) | 4 | Advanced FortiGate firewall administration |
| Palo Alto PCNSA | 4 | Palo Alto firewall administration |
| EC-Council Certified Network Defender (CND) | 4 | Defensive network security and hardening |
| Microsoft AZ-700 | 4 | Azure networking and hybrid connectivity |

---

## Advanced Level

| Cert | Importance | Notes |
|---|---|---|
| Palo Alto PCNSE | 5 | Enterprise firewall engineering and troubleshooting |
| AWS Advanced Networking – Specialty | 5 | Advanced AWS networking and hybrid cloud |
| GIAC Security Essentials (GSEC) | 4 | Enterprise security and networking |
| GIAC Certified Intrusion Analyst (GCIA) | 4 | IDS, packet analysis, and intrusion detection |
| GIAC Certified Incident Handler (GCIH) | 4 | Incident response and attack handling |
| CISSP (ISC2) | 5 | Global standard for security professionals |
| CCSP (ISC2) | 4 | Cloud security architecture and operations |
| CISM (ISACA) | 4 | Security management and governance |

---


# 3. Network Connections

Network connections define how devices are physically and logically connected to communicate and share data across a network.

---

## 3.1 Wired Networks

Wired networks use physical cables to connect devices.

### Types:
- Ethernet (most common)
- Fiber Optic (high speed, long distance)

### Features:
- Stable connection
- High speed
- Low interference
- Requires physical setup

---

## 3.2 Wireless Networks

Wireless networks use radio signals instead of cables.

### Types:
- Wi-Fi
- Bluetooth
- Mobile networks (4G/5G)

### Features:
- Flexible mobility
- Easy setup
- Can be affected by interference and range limits

---

## 3.3 VPN (Virtual Private Network)

A VPN creates a secure encrypted tunnel over a public network.

### Key Points:
- Hides user IP address
- Encrypts data traffic
- Used for privacy and secure communication

### Use Cases:
- Secure remote access
- Bypassing restrictions
- Safe browsing on public networks

---

## 3.4 VLAN (Virtual Local Area Network)

A VLAN logically divides a physical network into multiple virtual networks.

### Key Points:
- Improves network segmentation
- Enhances security
- Reduces broadcast traffic

### Example:
- HR department network separated from IT department on same physical switch

---

## 3.5 Subnetting Basics

Subnetting divides a large network into smaller networks.

### Why Subnetting?
- Efficient IP usage
- Better network performance
- Improved security isolation

### Key Concepts:
- IP Address
- Subnet Mask
- Network ID
- Host ID

### Example:
A large network split into:
- Subnet A (HR)
- Subnet B (Finance)
- Subnet C (IT)

---



# Router

## Definition

A **Router** is a Layer 3 (Network Layer) networking device that connects two or more different networks and forwards data packets between them using IP addresses. It determines the best path for data to travel from the source network to the destination network.

Routers are commonly used to connect Local Area Networks (LANs) to Wide Area Networks (WANs), such as the Internet.

## Functions

- Connects different networks together.
- Uses IP addresses to forward packets.
- Selects the best route using routing tables.
- Enables communication between LAN and Internet.
- Supports Network Address Translation (NAT).
- Can provide DHCP services.
- Helps reduce unnecessary network traffic.

## Advantages

- Connects multiple networks.
- Improves network management.
- Provides Internet connectivity.
- Supports advanced security features.
- Can connect wired and wireless networks.

## Disadvantages

- More expensive than switches.
- Configuration can be complex.
- Packet forwarding is slower than switching.

## Real-World Example

A home Wi-Fi router connects all devices in your house to your Internet Service Provider (ISP), allowing users to browse the Internet.

---

# Switch

## Definition

A **Switch** is a Layer 2 (Data Link Layer) networking device that connects multiple devices within the same Local Area Network (LAN). It forwards data using MAC addresses, ensuring that data reaches only the intended device.

Unlike hubs, switches reduce unnecessary traffic by sending frames only to the correct destination.

## Functions

- Connects devices in a LAN.
- Learns and stores MAC addresses.
- Forwards data only to the destination device.
- Reduces network collisions.
- Improves network performance.
- Supports VLANs in managed switches.

## Advantages

- High-speed communication.
- Efficient data forwarding.
- Reduces collisions.
- Better bandwidth utilization.
- Easy to expand the network.

## Disadvantages

- Cannot route traffic between different networks.
- Managed switches require configuration.
- More expensive than hubs.

## Real-World Example

A company uses a switch to connect computers, printers, IP phones, and servers within the same office.

---

# Firewall

## Definition

A **Firewall** is a network security device that monitors, filters, and controls incoming and outgoing network traffic based on predefined security rules. It acts as a barrier between trusted and untrusted networks.

Firewalls can be hardware-based, software-based, or cloud-based.

## Functions

- Blocks unauthorized access.
- Filters network traffic.
- Monitors incoming and outgoing connections.
- Prevents cyber attacks.
- Controls access based on security policies.
- Logs network activities.

## Advantages

- Improves network security.
- Prevents unauthorized access.
- Protects against malware.
- Helps enforce organizational security policies.
- Monitors suspicious traffic.

## Disadvantages

- Incorrect configuration may block legitimate traffic.
- Cannot stop every type of cyber attack.
- May introduce slight network latency.

## Real-World Example

A company firewall blocks malicious traffic from the Internet while allowing employees to securely access business applications.

---

# IDS (Intrusion Detection System)

## Definition

An **Intrusion Detection System (IDS)** continuously monitors network traffic and system activities to identify suspicious behavior, security policy violations, or cyber attacks. IDS only detects threats and generates alerts; it does not block them.

## Functions

- Monitors network traffic.
- Detects suspicious activities.
- Generates security alerts.
- Records attack logs.
- Helps security teams investigate incidents.

## Advantages

- Early threat detection.
- Improves network visibility.
- Assists in security monitoring.
- Provides detailed attack logs.

## Disadvantages

- Does not stop attacks automatically.
- Can generate false positives.
- Requires continuous monitoring.

## Real-World Example

An IDS detects repeated login attempts from an unknown IP address and alerts the security administrator.

---

# IPS (Intrusion Prevention System)

## Definition

An **Intrusion Prevention System (IPS)** detects malicious activities like an IDS but also takes automatic action to prevent attacks by blocking malicious traffic in real time.

## Functions

- Detects attacks.
- Blocks malicious packets.
- Prevents exploitation.
- Stops known vulnerabilities.
- Protects critical systems.

## Advantages

- Automatic threat prevention.
- Reduces attack impact.
- Improves overall network security.
- Responds in real time.

## Disadvantages

- Incorrect rules may block legitimate traffic.
- Requires frequent updates.
- Can slightly affect network performance.

## Real-World Example

An IPS automatically blocks an attacker attempting to exploit a known web server vulnerability.

---

# Access Point (AP)

## Definition

An **Access Point (AP)** is a networking device that provides wireless connectivity by allowing Wi-Fi-enabled devices to connect to a wired network. It extends network coverage and enables multiple wireless users to access the network simultaneously.

## Functions

- Provides Wi-Fi connectivity.
- Extends wireless coverage.
- Connects wireless devices to LAN.
- Supports multiple users.
- Improves wireless network availability.

## Advantages

- Wireless mobility.
- Easy device connectivity.
- Supports many users.
- Extends network coverage.
- Simple installation.

## Disadvantages

- Wireless interference.
- Limited range.
- Security must be properly configured.

## Real-World Example

A university installs multiple access points throughout the campus to provide Wi-Fi access for students and faculty.

---

# Load Balancer

## Definition

A **Load Balancer** is a networking device or software that distributes incoming client requests across multiple servers. This ensures no single server becomes overloaded and improves application performance, scalability, and availability.

## Functions

- Distributes network traffic.
- Prevents server overload.
- Improves application performance.
- Ensures high availability.
- Supports failover if a server becomes unavailable.

## Advantages

- Better performance.
- High availability.
- Improved scalability.
- Increased reliability.
- Better user experience.

## Disadvantages

- Additional deployment cost.
- Requires proper configuration.
- Can become a single point of failure if not deployed redundantly.

## Real-World Example

Large websites such as Amazon, Netflix, and Google use load balancers to distribute millions of user requests across multiple servers, ensuring fast response times and continuous service.

# SkillMate - Network Security Learning Pathway

> Learn Networking → Understand Security → Practice in Labs → Solve Challenges → Prepare for Certifications → Become Job Ready

---

# Phase 0 - Welcome

- Introduction to Network Security
- How to use this pathway
- Career Roadmap
- Required Software
- Lab Setup
- Learning Methodology

---

# Phase 1 - Networking Fundamentals

- What is a Network?
- Types of Networks
- Network Topologies
- OSI Model
- TCP/IP Model
- Data Encapsulation
- Packet Flow
- Network Communication
- Bandwidth
- Latency
- MTU

---

# Phase 2 - Network Devices

- Router
- Switch
- Hub
- Bridge
- Repeater
- Gateway
- Firewall
- Access Point
- Modem
- Load Balancer
- IDS
- IPS

 Build Your First Network

---

# Phase 3 - IP Addressing

- IPv4
- IPv6
- MAC Address
- Public & Private IP
- CIDR
- Subnetting
- Supernetting
- NAT
- PAT

 Subnetting Labs

---

# Phase 4 - Network Protocols

- ARP
- ICMP
- TCP
- UDP
- DNS
- DHCP
- HTTP
- HTTPS
- FTP
- SSH
- SMTP
- POP3
- IMAP
- SNMP
- LDAP
- SMB
- RDP

 Packet Analysis Labs

---

# Phase 5 - Network Services

- DNS
- DHCP
- NTP
- Proxy
- VPN
- Directory Services

---

# Phase 6 - Routing & Switching

- Routing Basics
- Static Routing
- Dynamic Routing
- OSPF
- BGP
- VLAN
- STP
- RSTP
- EtherChannel

 Cisco Packet Tracer Labs

---

# Phase 7 - Network Security Fundamentals

- CIA Triad
- AAA
- Authentication
- Authorization
- Accounting
- Least Privilege
- Zero Trust
- Network Segmentation
- Defense in Depth
- Security Policies

---

# Phase 8 - Firewalls

- Packet Filtering
- Stateful Firewall
- NGFW
- WAF
- ACL
- Firewall Rules
- Firewall Policies

Configure Firewall Rules

---

# Phase 9 - VPN & Remote Access

- VPN Basics
- IPSec
- SSL VPN
- Site-to-Site VPN
- Remote Access VPN
- Split Tunnel
- Full Tunnel

---

# Phase 10 - Wireless Security

- Wi-Fi Basics
- WPA2
- WPA3
- Enterprise Wi-Fi
- Rogue AP
- Evil Twin
- Deauthentication Attack

---

# Phase 11 - Network Attacks

- ARP Spoofing
- DNS Poisoning
- MAC Flooding
- MITM
- VLAN Hopping
- DHCP Starvation
- Session Hijacking
- DDoS
- Packet Sniffing


---

# Phase 12 - Wireshark

- Installation
- Packet Capture
- Filters
- TCP Analysis
- DNS Analysis
- HTTP Analysis
- Troubleshooting
- Enterprise Investigation

---

# Phase 13 – Network Scanning & Enumeration

Learn how to discover hosts, identify open ports, detect running services, fingerprint operating systems, and perform large-scale network scanning.

## Tools
- Nmap
- Masscan

## Topics
- Installation
- Host Discovery
- Port Scanning
- Service Detection
- Version Detection
- NSE (Nmap Scripting Engine)
- OS Detection
- Host Enumeration
- Banner Grabbing
- Scan Optimization
- Timing Templates
- Firewall Evasion Basics
- Output Formats
- Scan Analysis

---

# Phase 14 – Network Traffic Analysis

Learn how to capture, filter, inspect, and analyze network packets for troubleshooting and security analysis.

## Tools
- tcpdump
- TShark

## Topics
- Packet Capturing
- Capture Filters
- Display Filters
- Exporting PCAP Files
- Packet Inspection
- Protocol Analysis
- Traffic Analysis
- Flow Analysis
- Network Troubleshooting
- Command-Line Packet Analysis

---

# Phase 15 – Network Connectivity & Troubleshooting

Learn how to test connectivity, verify communication, and troubleshoot network issues.

## Tools
- Ping
- Traceroute
- Netcat

## Topics
- ICMP
- Connectivity Testing
- Latency Testing
- Packet Loss Analysis
- Route Discovery
- Hop Analysis
- Banner Grabbing
- TCP Client & Server
- UDP Communication
- File Transfer
- Port Testing
- Network Troubleshooting

---

# Phase 16 – DNS Analysis & Troubleshooting

Learn how the Domain Name System works and how to query DNS servers.

## Tools
- nslookup
- dig

## Topics
- DNS Queries
- Forward Lookup
- Reverse Lookup
- A Records
- AAAA Records
- MX Records
- TXT Records
- NS Records
- CNAME Records
- SOA Records
- Advanced Queries
- DNS Troubleshooting

---

# Phase 17 – Network Interface & Socket Management

Learn how to configure network interfaces, manage routes, inspect sockets, and monitor active connections.

## Tools
- ip
- ifconfig
- netstat
- ss
- arp

## Topics
- Interface Management
- IP Address Configuration
- Routing Tables
- Default Gateway
- ARP Cache
- Socket Analysis
- Active Connections
- Listening Ports
- Process Mapping
- Network Statistics
- Interface Monitoring

---

# Phase 18 – Web Communication & File Transfer

Learn how to communicate with web servers, test APIs, and automate downloads.

## Tools
- curl
- wget

## Topics
- HTTP Requests
- HTTPS Requests
- REST APIs
- HTTP Methods
- Request Headers
- Authentication
- Cookies
- File Downloads
- Resume Downloads
- Automation
- Script Integration

---

# Phase 19 – Encryption & Network Performance

Learn the basics of encryption, SSL/TLS certificates, and network performance testing.

## Tools
- OpenSSL
- iperf3

## Topics
- SSL/TLS
- X.509 Certificates
- Certificate Inspection
- Public & Private Keys
- Encryption
- Hashing
- CSR Generation
- Bandwidth Testing
- Throughput Analysis
- Latency Measurement
- Network Performance Analysis

---

# Phase 20 – Packet Crafting & Automation

Learn how to build, modify, send, receive, and automate custom network packets.

## Tools
- Scapy

## Topics
- Packet Crafting
- Packet Sniffing
- Packet Injection
- Packet Manipulation
- Custom Protocols
- Network Automation
- Python Scripting
- Security Testing
- Protocol Analysis

---

# Phase 21 – Man-in-the-Middle (MITM) & Network Attacks

Learn how interception attacks work in authorized lab environments.

## Tools
- Bettercap
- Ettercap

## Topics
- MITM Fundamentals
- Network Discovery
- ARP Spoofing
- DNS Spoofing
- Packet Forwarding
- Packet Injection
- Credential Capture (Lab)
- Traffic Interception
- Session Analysis
- Network Reconnaissance

---

# Phase 22 – Web Server Security Assessment

Learn how to identify web server vulnerabilities and security misconfigurations.

## Tools
- Nikto

## Topics
- Web Server Scanning
- Vulnerability Detection
- Misconfiguration Detection
- SSL Testing
- CGI Enumeration
- Security Headers
- Report Generation
- Web Security Assessment

---

# Phase 23 – Network Monitoring & Intrusion Detection

Learn how organizations monitor network traffic and detect malicious activity.

## Tools
- Zeek
- Snort
- Suricata

## Topics
- Network Monitoring
- Network Security Monitoring (NSM)
- Intrusion Detection Systems (IDS)
- Intrusion Prevention Systems (IPS)
- Signature-Based Detection
- Rule Creation
- Protocol Analysis
- Threat Detection
- Alert Generation
- Log Analysis
- Event Correlation
- Network Forensics

# Phase 24 - ARP Tool

- Cache
- Troubleshooting

---

# Phase 25 - curl

- HTTP Requests
- APIs
- Testing

---

# Phase 26 - wget

- Downloads
- Automation

---

# Phase 27 - OpenSSL

- Certificates
- TLS
- Encryption

---

# Phase 28 - iperf3

- Bandwidth Testing
- Performance Analysis

---

# Phase 29 - TShark

- CLI Packet Analysis

---

# Phase 30 - Scapy

- Packet Crafting
- Packet Automation

---

# Phase 31 - Bettercap

- MITM Framework
- Network Discovery

---

# Phase 32 - Ettercap

- MITM
- ARP Spoofing

---

# Phase 33 - Masscan

- High-Speed Network Scanning

---

# Phase 34 - Nikto

- Web Server Scanning

---

# Phase 35 - Zeek

- Network Monitoring
- Logs
- Detection

---

# Phase 36 - Snort

- IDS
- Rules
- Detection

---

# Phase 37 - Suricata

- IDS/IPS
- Threat Detection

---

# Phase 38 - Enterprise Networking

- Active Directory
- DNS Infrastructure
- DHCP Infrastructure
- Proxy Servers
- NAC
- Enterprise VLAN Design

---

# Phase 39 - Cloud Networking

- AWS VPC
- Azure VNet
- Security Groups
- NACL
- Route Tables
- VPN Gateway

---

# Phase 40 - SIEM Integration

- Syslog
- Zeek Logs
- Suricata Logs
- Splunk
- Microsoft Sentinel
- QRadar

---

# Phase 41 - Labs

- Cisco Packet Tracer
- GNS3
- EVE-NG
- VirtualBox
- VMware

Enterprise Scenarios

---

# Phase 43 - Certifications

## Beginner
- Cisco CCST Networking
- Cisco CCNA
- CompTIA Network+

## Intermediate
- CompTIA Security+
- Cisco CyberOps Associate
- Cisco DevNet Associate
- Fortinet FCA
- Fortinet FCP
- Palo Alto PCCET
- Palo Alto PCNSA

## Advanced
- Cisco CCNP Enterprise
- Cisco CCNP Security
- GIAC GCIA
- GIAC GSEC
- EC-Council CND
- OffSec OSCP
- CISSP

## Phase 44 - Ports & Network Services 
- What are Ports?
- What is a Port?
- Why Ports Exist
- Port Numbers
- Client Port vs Server Port
- Ephemeral Ports
- Well Known Ports
- Registered Ports
- Dynamic Ports
- TCP Ports
- UDP Ports
- Socket Basics
- Port States
- Listening vs Established Ports


#  Network Security & Penetration Testing – Index

---

## 1. Network Architecture
- Network Models (LAN, WAN, MAN, Hybrid)
- OSI Model
- TCP/IP Model
- Network Communication Flow

---

## 2. Network Devices
- Router
- Switch
- Firewall
- IDS / IPS
- Access Points
- Load Balancers

---

## 3. Network Connections
- Wired Networks
- Wireless Networks
- VPN
- VLAN
- Subnetting Basics

---

## 4. IP Addressing & Routing
- IPv4 Addressing
- IPv6 Addressing
- Subnetting
- CIDR
- Routing Basics
- NAT (Network Address Translation)

---

## 5. Network Protocols
- HTTP / HTTPS
- DNS
- DHCP
- TCP / UDP
- ICMP
- FTP / SFTP
- SSH
- SMB
- SMTP / IMAP / POP3

---

## 6. Security Principles
- CIA Triad
- Authentication & Authorization
- Threats, Vulnerabilities, Exploits
- Security Layers

---

## 7. Network Attacks
- Reconnaissance Attacks
- Scanning Attacks
- Man-in-the-Middle (MITM)
- Sniffing & Spoofing
- Brute Force Attacks
- Credential Attacks
- Enumeration Attacks
- Service Exploitation

---

## 8. Vulnerabilities
- Open Ports
- Default Credentials
- Weak Passwords
- Misconfigurations
- Unpatched Services
- Information Leakage

---

## 9. Port-Based Security Checklist
- Port 21 – FTP
  - Anonymous login (anonymous/anonymous)
  - Default credentials testing
  - Username enumeration
  - File upload/download testing
  - Misconfiguration checks

---

## 10. Reconnaissance & Enumeration
- Network Scanning
- Service Enumeration
- Username Enumeration
- Banner Grabbing
- OS & Service Detection
- SMB / FTP / SSH Enumeration

---

## 11. Exploitation Tools

### Metasploit Framework
- msfconsole
- search
- use
- set / unset
- exploit / run
- meterpreter
- db_* commands
- Multi-target handling

### Hydra
- Brute force attacks
- Username enumeration
- Password attacks
- Protocol-based attacks (FTP, SSH, HTTP)

---

## 12. Password Attacks
- Brute Force Attacks
- Dictionary Attacks
- Credential Stuffing
- Default Credential Testing
- Password Spraying

---

## 13. Pentesting Workflow
- Reconnaissance
- Scanning
- Enumeration
- Exploitation
- Privilege Escalation
- Post Exploitation

---




## Definition

The **CIA Triad** is the fundamental security model in cybersecurity and serves as the foundation for protecting information systems. It consists of three core principles: **Confidentiality**, **Integrity**, and **Availability**. These principles help organizations design secure systems, implement security policies, and evaluate the effectiveness of security controls.

### Confidentiality

**Confidentiality** ensures that sensitive information is accessible only to authorized users and protected from unauthorized disclosure. Organizations achieve confidentiality through techniques such as encryption, authentication, authorization, access control lists (ACLs), data classification, and Multi-Factor Authentication (MFA).

### Integrity

**Integrity** ensures that data remains accurate, consistent, complete, and unaltered throughout its lifecycle. Any unauthorized modification, deletion, or corruption of data should be prevented or detected. Common mechanisms used to maintain integrity include hashing algorithms, digital signatures, checksums, version control, and file integrity monitoring.

### Availability

**Availability** ensures that systems, services, applications, and data are accessible whenever authorized users need them. Organizations maintain availability through redundancy, backups, disaster recovery planning, load balancing, failover systems, regular maintenance, and protection against Denial-of-Service (DoS) attacks.

The CIA Triad is widely used when designing secure applications, performing risk assessments, and developing cybersecurity strategies.

---

# Authentication & Authorization

## Definition

**Authentication** is the process of verifying the identity of a user, device, application, or service before granting access to a system. It answers the question, **"Who are you?"** Authentication ensures that only legitimate users can access protected resources.

Common authentication methods include:

- Username and Password
- PIN
- Biometrics (Fingerprint, Face Recognition, Iris Scan)
- Smart Cards
- Security Tokens
- Multi-Factor Authentication (MFA)

**Authorization** is the process of determining what an authenticated user is permitted to access or perform within a system. It answers the question, **"What are you allowed to do?"** Authorization is enforced through permissions, user roles, security policies, and access control mechanisms such as Role-Based Access Control (RBAC) and Attribute-Based Access Control (ABAC).

Authentication always occurs before authorization. Without successful authentication, authorization cannot be performed.

---

# Threats, Vulnerabilities, Exploits

## Definition

Understanding the relationship between **Threats**, **Vulnerabilities**, and **Exploits** is one of the most important concepts in cybersecurity because most cyber attacks involve all three components.

### Threat

A **Threat** is any potential danger capable of causing damage to an organization's systems, networks, or information. Threats may come from cybercriminals, insider attacks, malware, ransomware, phishing campaigns, social engineering, natural disasters, or accidental human errors.

### Vulnerability

A **Vulnerability** is a weakness or flaw in software, hardware, operating systems, applications, network devices, or security processes that can be exploited by an attacker. Vulnerabilities often result from software bugs, outdated systems, weak passwords, insecure configurations, or missing security patches.

### Exploit

An **Exploit** is the technique, program, or piece of code used by an attacker to take advantage of a vulnerability. Successful exploitation can lead to unauthorized access, privilege escalation, malware installation, data theft, or complete system compromise.

Organizations reduce risk by identifying vulnerabilities through security assessments, applying software updates, implementing security controls, and continuously monitoring their infrastructure.

---

# Security Layers (Defense in Depth)

## Definition

**Security Layers**, commonly known as **Defense in Depth**, is a cybersecurity strategy that protects systems by implementing multiple independent layers of security controls. Instead of relying on a single security solution, organizations deploy several defensive mechanisms so that if one layer is compromised, additional layers continue protecting critical assets.

Defense in Depth combines **physical**, **administrative**, and **technical** security controls to create a comprehensive security architecture.

Common security layers include:

- Physical Security
- Network Security
- Endpoint Security
- Application Security
- Identity and Access Management (IAM)
- Firewalls
- Intrusion Detection and Prevention Systems (IDS/IPS)
- Encryption
- Antivirus and Anti-malware Protection
- Security Monitoring and Logging
- Backup and Disaster Recovery
- Security Awareness Training

By implementing multiple security layers, organizations can reduce attack surfaces, detect threats earlier, minimize the impact of security incidents, and improve overall cyber resilience. Defense in Depth is considered one of the most effective approaches for protecting modern enterprise networks and information systems.



