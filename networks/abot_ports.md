# Commonly Asked Ports in Interviews

## Introduction to Ports
Ports are logical communication endpoints that allow applications and services to exchange data over a network. Each port is identified by a **port number** ranging from **0 to 65535**, divided into specific categories based on their use cases. Understanding these categories is crucial for networking and cybersecurity interviews.

### Port Ranges and Categories
1. **Reserved Ports (0–1023)**   
   - **Purpose**: Reserved for essential system services and widely used protocols such as HTTP, FTP, and SSH. These ports are assigned and maintained by the **Internet Assigned Numbers Authority (IANA)**.   

2. **Registered Ports (1024–49151)**  
   - **Purpose**: Used by user-defined or application-specific services and processes. These ports are not as standardized as reserved ports but are registered with IANA to avoid conflicts. They are commonly used by applications such as databases and custom software.  

3. **Dynamic/Private Ports (49152–65535)**  
   - **Also Known As**: Ephemeral Ports.  
   - **Purpose**: Assigned dynamically by the operating system for short-lived connections, typically client-side. These ports are used for outbound connections and are not permanently assigned to any service.  
   
### Total Number of Ports
- **Total Ports**: 65,536 (0–65535).  
- **Reserved Ports**: Ports 0–1023 are set aside for widely used and critical protocols.  
- **Dynamic Ports**: These are temporary and vary between sessions, supporting scalability for multiple simultaneous connections.  

---

## Well-Known Ports (0–1023)
### Networking Protocols
| **Port** | **Protocol**        | **Description**                                   |
|----------|---------------------|---------------------------------------------------|
| 20, 21   | FTP                 | File Transfer Protocol (20: Data, 21: Control).  |
| 22       | SSH                 | Secure Shell for secure logins and file transfers. |
| 23       | Telnet              | Unsecure remote terminal access.                 |
| 25       | SMTP                | Simple Mail Transfer Protocol (email sending).   |
| 53       | DNS                 | Domain Name System (resolves domain names).      |
| 67, 68   | DHCP                | Dynamic Host Configuration Protocol.             |
| 69       | TFTP                | Trivial File Transfer Protocol (simple file transfer). |
| 80       | HTTP                | HyperText Transfer Protocol (web traffic).       |
| 110      | POP3                | Post Office Protocol (email retrieval).          |
| 119      | NNTP                | Network News Transfer Protocol.                  |
| 123      | NTP                 | Network Time Protocol (time synchronization).    |
| 143      | IMAP                | Internet Message Access Protocol (email retrieval). |
| 161, 162 | SNMP                | Simple Network Management Protocol.              |
| 389      | LDAP                | Lightweight Directory Access Protocol.           |
| 443      | HTTPS               | HTTP Secure (encrypted web traffic).             |
| 445      | SMB/CIFS            | Server Message Block/Common Internet File System. |

---

## Registered Ports (1024–49151)
### Application-Specific Protocols
| **Port** | **Protocol**        | **Description**                                   |
|----------|---------------------|---------------------------------------------------|
| 3306     | MySQL               | MySQL database system.                           |
| 3389     | RDP                 | Remote Desktop Protocol.                         |
| 5432     | PostgreSQL          | PostgreSQL database system.                      |
| 8080     | HTTP Proxy          | Alternative HTTP or proxy servers.               |
| 8443     | HTTPS Proxy         | Secure alternative for HTTP.                     |

---

## Dynamic/Private Ports (49152–65535)
- **Ephemeral Ports**: Used for dynamic port allocations in communications initiated by the client.
- **Example Use**: Temporary ports for outbound connections like web browsing.
- **Characteristics**:  
  - Assigned dynamically and released when no longer in use.  
  - Common in high-volume systems with multiple concurrent sessions.  

---

## Security and Administrative Ports
| **Port** | **Protocol**        | **Description**                                   |
|----------|---------------------|---------------------------------------------------|
| 135      | RPC                 | Remote Procedure Call.                           |
| 137–139  | NetBIOS             | Network Basic Input/Output System.               |
| 1521     | Oracle DB           | Oracle Database default listener.                |
| 1433,1434| MS SQL Server       | Microsoft SQL Server (database service).         |
| 4444     | Metasploit          | Default port for exploits in Metasploit.         |  

---

This guide provides a detailed overview of commonly asked ports, their classification, and their significance in networking and cybersecurity interviews.
