# My CompTIA Network+ (N10-009) Learning Journey

Welcome! This repository is my active learning log as I build a foundational knowledge of networking. I am currently following Professor Messer's CompTIA N10-009 training course.

My goal is not just to learn the concepts, but to understand how they apply in real-world scenarios, especially in my future career in cybersecurity.

---

## 🗓️ Learning Log

### November 7, 2025: The Foundation
* **Topics Covered:** The theoretical blueprints for all network communication.
* **Messer Modules:** 1.1 (The OSI Model & TCP/IP)
* **Key Takeaway:** The OSI model is the "why" (theory), and the TCP/IP model is the "how" (practical). Understanding the layers helps in troubleshooting—is this a Layer 1 (cable) problem or a Layer 3 (IP) problem?

### November 8, 2025: Hardware, Functions, and Ports
* **Topics Covered:** A dense day covering the core components of a network and how they communicate.
* **Messer Modules:** 1.2 (Network Devices & Functions) & 1.4 (Ports & Protocols)
* **Key Takeaway:** I'm starting to see the network less as a "cloud" and more as a physical system of hardware (devices) running specific services (protocols) that are only accessible through designated doors (ports).

---

## 🧠 Key Concepts Covered (So Far)

### 1. Network Models: The Blueprints
This is the core theory of how devices "talk" to each other. The 7-layer **OSI Model** is perfect for understanding the theory, while the 4-layer **TCP/IP Model** is what we actually use.



[Image of OSI Model vs TCP/IP Model mapping]


### 2. Network Devices: The Hardware
These are the physical components that build the network.
* **Core:**
    * **Router:** The "post office" that directs traffic *between* different networks. Operates at OSI Layer 3.
    * **Switch:** The "local mail carrier" that directs traffic *within* the same network. Operates at OSI Layer 2.
* **Security:**
    * **Firewall:** A "security guard" that filters traffic based on a set of rules (e.g., ports, IPs).
    * **IDS (Intrusion Detection System):** A "security camera" that logs suspicious activity.
    * **IPS (Intrusion Prevention System):** An "armed guard" that can actively *stop* suspicious activity.
* **Efficiency & Services:**
    * **Load Balancer:** A "traffic cop" that distributes requests across multiple servers so no single one gets overwhelmed.
    * **Proxy Server:** A "middle-man" that makes requests on your behalf, hiding your real IP.
* **Storage:**
    * **NAS (Network Attached Storage):** A simple "file server" on the network. Easy to use.
    * **SAN (Storage Area Network):** A high-speed, dedicated *network* for storage. Much faster and more complex.
* **Wireless:**
    * **Access Point (AP):** The device that creates the Wi-Fi signal.
    * **Wireless LAN Controller (WLC):** The "manager" that controls many APs from one place (used in offices, schools).

### 3. Network Functions: The "Rules of the Road"
* **CDN (Content Delivery Network):** A "local warehouse" for web content. It stores copies of websites (like Netflix movies) all over the world so you can stream them faster.
* **VPN (Virtual Private Network):** Creates a secure, encrypted "tunnel" for your traffic.
* **QoS (Quality of Service):** A "priority lane" for important traffic (like a Zoom call) over less-important traffic (like a file download).
* **TTL (Time to Live):** A "self-destruct timer" on a data packet to prevent it from getting stuck in an infinite routing loop.

### 4. Ports & Protocols: The Doors & Languages
This is the most critical part for my cybersecurity goals. A port is the "door" a service listens on, and the protocol is the "language" it speaks. Here are the common ones, grouped by their job. (Based on Messer 1.4)

#### 🌐 Web & Remote Access
* **Port 80 (HTTP):** Unencrypted web.
* **Port 443 (HTTPS):** Encrypted web (uses SSL/TLS).
* **Port 22 (SSH):** **Secure Shell**. Encrypted command-line for remote login.
* **Port 23 (Telnet):** *Unencrypted* command-line. A major security risk.
* **Port 3389 (RDP):** **Remote Desktop Protocol**. Graphical remote access for Windows.

#### 📁 File Transfer
* **Port 21 (FTP):** **File Transfer Protocol**. Old and *unencrypted*.
* **Port 22 (SFTP):** **Secure File Transfer Protocol**. Runs *inside* SSH. Encrypted.
* **Port 69 (TFTP):** **Trivial File Transfer**. Simple, *unencrypted*, and uses UDP. No authentication.
* **Port 445 (SMB):** **Server Message Block**. Windows file/printer sharing. A very common target.

#### ✉️ Email
* **Port 25 (SMTP):** **Simple Mail Transfer Protocol**. Used to *send* email between servers.
* **Port 143 (IMAP):** **Internet Message Access Protocol**. Used to *sync* email with a server (like Gmail).

#### 🏢 Core Infrastructure & Directory Services
* **Port 53 (DNS):** **Domain Name System**. The internet's "phonebook."
* **Ports 67/68 (DHCP):** **Dynamic Host Configuration Protocol**. Assigns IPs automatically.
* **Port 123 (NTP):** **Network Time Protocol**. Keeps all computer clocks in sync.
* **Port 389 (LDAP):** **Lightweight Directory Access Protocol**. An "address book" for user accounts.
* **Port 636 (LDAPS):** **LDAP over SSL**. The *secure*, encrypted version of LDAP.
* **Ports 161/162 (SNMP):** **Simple Network Management Protocol**. Used to monitor device health.

#### 🛢️ Databases
* **Port 1433 (MS-SQL):** Microsoft SQL Server.
* **Port 3306 (MySQL):** A very popular open-source database.
