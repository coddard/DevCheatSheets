# 🔧 Network Ports Cheat Sheet 🚀

A fun and non-exhaustive list of **network ports** used across different domains! Perfect for developers, sysadmins, and curious folks who want to know what port does what.

---

## 🌐 Web Ports 🌍

| Port | Name         | Description                       |
|------|--------------|-----------------------------------|
| 80   | HTTP         | HyperText Transfer Protocol       |
| 443  | HTTPS        | HTTP Secure (SSL/TLS)             |
| 8080 | HTTP-Alt     | Alternative HTTP Port             |
| 8443 | HTTPS-Alt    | Alternative HTTPS Port            |
| 8000 | HTTP-Proxy   | For proxy server HTTP             |
| 8008 | HTTP-Backup  | Backup port for HTTP              |
| 8888 | HTTP-Alternative | Alternative port for HTTP     |

---

## ⚙️ Network & Infrastructure Ports 🛰️

| Port | Name           | Description                             |
|------|----------------|-----------------------------------------|
| 53   | DNS            | Domain Name System 🪄                   |
| 67/68| DHCP           | Dynamic Host Configuration Protocol 🆔  |
| 123  | NTP            | Network Time Protocol ⏰                 |
| 161  | SNMP           | Simple Network Management Protocol 📶    |
| 162  | SNMP-Trap      | SNMP Trap Messages 🚨                  |
| 514  | Syslog         | Logging system 🗂️                       |
| 69   | TFTP           | Trivial File Transfer Protocol 📤       |

---

## 🐳 Virtualization & Containerization Ports 🧱

| Port | Name              | Description                        |
|------|-------------------|------------------------------------|
| 2375 | Docker (No TLS)   | Docker without TLS 🔓              |
| 2376 | Docker (TLS)      | Docker with TLS 🔒                 |
| 6443 | Kubernetes API    | Kubernetes API Server 🧭           |
| 8443 | Kubernetes Alt    | Alternative Kubernetes API port 🔄  |
| 9100 | Node Exporter     | Prometheus Node Exporter 📊        |
| 9090 | Prometheus        | Prometheus Monitoring 🕵️‍♂️         |
| 5672 | RabbitMQ          | Message Broker RabbitMQ 📮          |

---

## 📊 Monitoring & Management Ports 🧪

| Port | Name               | Description                          |
|------|--------------------|--------------------------------------|
| 631  | IPP                | Internet Printing Protocol 🖨️         |
| 873  | rsync              | Remote Sync 📁                        |
| 8086 | InfluxDB           | Time Series Database InfluxDB 💾      |
| 9093 | Prometheus Alert   | Prometheus Alertmanager 🚩            |

---

## 🗃️ Database Ports 🗄️

| Port | Name             | Description                           |
|------|------------------|---------------------------------------|
| 1433 | Microsoft SQL    | Microsoft SQL Database Server 🪑       |
| 3306 | MySQL            | MySQL Database Management System 🐬    |
| 5432 | PostgreSQL       | PostgreSQL DBMS 🧠                    |
| 1521 | Oracle           | Oracle Database Management System 💼   |
| 27017| MongoDB          | MongoDB NoSQL Database 🦖             |
| 11211| Memcached        | Memcached Memory Caching System ⚡     |
| 6379 | Redis            | Redis In-Memory Database 🧲           |

---

## 🖥️ Remote Communication Ports 🌐

| Port | Name   | Description                         |
|------|--------|-------------------------------------|
| 22   | SSH    | Secure Shell 🛡️                     |
| 23   | Telnet | Unsecure remote terminal protocol 🕳️ |
| 3389 | RDP    | Remote Desktop Protocol 🖥️           |
| 5900 | VNC    | Virtual Network Computing 🖽          |
| 179  | BGP    | Border Gateway Protocol 🧭           |
| 113  | Ident  | Ident Protocol 🆔                    |

---

## 📧 Email & Messaging Ports ✉️

| Port | Name            | Description                          |
|------|-----------------|--------------------------------------|
| 25   | SMTP            | Simple Mail Transfer Protocol 📨      |
| 465  | SMTPS           | SMTP Secure 🔒                       |
| 587  | SMTP-Submission | Port for email submission 💌         |
| 110  | POP3            | Post Office Protocol v3 📥           |
| 995  | POP3S           | POP3 Secure 🛡️                       |
| 143  | IMAP            | Internet Message Access Protocol 📬  |
| 993  | IMAPS           | IMAP Secure 🛡️                       |

---

## 🎤 VoIP & Instant Messaging Ports 🎙️

| Port | Name           | Description                               |
|------|----------------|-------------------------------------------|
| 5060 | SIP            | Session Initiation Protocol 🗣️            |
| 5061 | SIP-Secure     | SIP over TLS 🔒                           |
| 1720 | H.323          | VoIP communication protocol 📞           |
| 3478 | STUN           | NAT traversal utility 🧭                 |
| 1234 | Skype          | Skype communication port 🎯              |
| 5222 | XMPP           | Extensible Messaging Protocol 💬          |
| 5223 | XMPP-Secure    | XMPP over SSL 🔐                         |

---

## 🎥 Streaming & Real-Time Media Ports 🎥

| Port       | Name   | Description                                  |
|------------|--------|----------------------------------------------|
| 5004       | RTP    | Real-time Transport Protocol for media 🎞️   |
| 9000       | WebRTC | Browser-based real-time communication 🖥️    |
| 16384–32767| RTP    | Range for dynamic audio/video streams 🎧    |

---

## 📦 P2P & File Sharing Ports 📦

| Port       | Name       | Description                                |
|------------|------------|--------------------------------------------|
| 6881–6889  | BitTorrent | Used by BitTorrent clients 🧲              |
| 51413      | BitTorrent | Default BitTorrent port 📡                 |
| 6969       | BitTorrent Tracker | BitTorrent tracker port 📍        |
| 1194       | OpenVPN    | Also used in P2P sharing 🧴                |
| 4661       | uTorrent   | Specific to uTorrent client 🐢             |
| 37152      | Steam      | Game downloads via Steam platform 🎮       |

---

## 🔒 Security & Tunneling Ports 🛡️

| Port | Name          | Description                              |
|------|---------------|------------------------------------------|
| 1194 | OpenVPN       | Virtual Private Network 🧴                |
| 1701 | L2TP          | Layer 2 Tunneling Protocol 📦             |
| 1723 | PPTP          | Point-to-Point Tunneling Protocol 🌀       |
| 4500 | IPsec-NAT-T   | IPsec NAT Traversal 🧱                    |
| 500  | IKE           | Internet Key Exchange 🔐                  |
| 1812 | RADIUS        | Authentication service 🔐                 |
| 3306 | MySQL SSL     | MySQL with SSL encryption 🔒              |

---

## 🔐 Cryptography & SSL/TLS Ports 🔒

| Port | Name      | Description                            |
|------|-----------|----------------------------------------|
| 443  | HTTPS     | HTTP Secure with SSL/TLS 🔒             |
| 993  | IMAPS     | IMAP secure with SSL/TLS 🛡️             |
| 995  | POP3S     | POP3 secure with SSL/TLS 🛡️             |
| 636  | LDAPS     | LDAP secure with SSL/TLS 🔐              |
| 8443 | HTTPS-Alt | Alternative HTTPS port 🔄                |
| 8888 | SSL Proxy | Secure proxy using SSL/TLS 🔒            |
| 563  | SNEWS     | Secure Network News Transfer Protocol 📰 |

---

## 📁 File Transfer & Share Ports 📤

| Port | Name         | Description                         |
|------|--------------|-------------------------------------|
| 20   | FTP-DATA     | FTP data transfer 📤                |
| 21   | FTP          | File Transfer Protocol 📁            |
| 22   | SFTP         | Secure File Transfer Protocol 🔒     |
| 445  | SMB          | Windows Shares 🪟                    |
| 139  | NetBIOS-SSN  | NetBIOS session service 🖥️           |
| 2049 | NFS          | Unix/Linux file sharing 🐧           |
| 548  | AFP          | Apple Filing Protocol 🍏              |

---

## 🎮 Gaming & Entertainment Ports 🎮

| Port   | Name       | Description                          |
|--------|------------|--------------------------------------|
| 27015  | Steam      | Steam gaming platform 🎮              |
| 7777   | Unreal Engine | Game servers using Unreal Engine 🎮 |
| 27020  | Source Engine | Game servers using Source Engine 🎮 |
| 28910  | Various Games | Multiplayer games 🎲                |
| 27000  | Various Games | Additional multiplayer games 🎲     |

---

## 🎁 Miscellaneous Service Ports 🎁

| Port   | Name       | Description                           |
|--------|------------|---------------------------------------|
| 500    | ISAKMP     | Security association setup 🔐          |
| 520    | RIP        | Routing Information Protocol 🧭        |
| 1900   | UPnP       | Plug-and-play device discovery 🔌     |
| 3659   | RADIUS     | Remote authentication service 🔐      |

---

## 🙌 Contribution

Found a missing port? Want to add more services or emojis?

👉 Fork this repo and send a PR!

---

## 📝 License

MIT License – feel free to use and remix!