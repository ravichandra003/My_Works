# **IP Address Overview**

An **IP address** is a unique identifier assigned to devices connected to a network. It allows devices to communicate with each other by sending and receiving data over the internet or a local network.

---

## **Types of IP Addresses**

### 1. **Based on Protocol**
- **IPv4 (Internet Protocol version 4)**:
  - Format: Four decimal numbers separated by dots (e.g., `192.168.1.1`).
  - Total Addresses: ~4.3 billion (32-bit address space).
  - Example: `192.0.2.1`, `8.8.8.8`.

- **IPv6 (Internet Protocol version 6)**:
  - Format: Eight groups of hexadecimal numbers separated by colons (e.g., `2001:0db8:85a3:0000:0000:8a2e:0370:7334`).
  - Total Addresses: ~340 undecillion (128-bit address space).
  - Example: `2001:db8::ff00:42:8329`
  - The double colon (::) is a shorthand to represent consecutive groups of zeroes. It can appear only once in an IPv6 address.

### 2. **Based on Scope**
- **Public IP Address**:
  - Globally unique and assigned by an ISP.
  - Used for communication over the internet.
  - Example: `123.45.67.89`.

- **Private IP Address**:
  - Used within local networks; not routable on the internet.
  - Reserved ranges:
    - IPv4: `10.0.0.0/8(large organisation)`, `172.16.0.0/12(mid)`, `192.168.0.0/16(home)`.
    - IPv6: `fd00::/8` (Unique Local Address).

### 3. **Special-Purpose IP Addresses**
- **Loopback Address**:
  - Used for testing; refers to the device itself.
  - IPv4: `127.0.0.1`.
  - IPv6: `::1`.

- **Multicast Address**:
  - Used for delivering packets to a group of devices.
  - IPv4: `224.0.0.0/4`.
  - IPv6: `ff00::/8`.

- **Broadcast Address**:
  - Sends data to all devices in a network.
  - Example: `192.168.1.255` for a `192.168.1.0/24` subnet.

- **APIPA (Automatic Private IP Addressing)**:
  - Used when a device cannot obtain an IP from a DHCP server.
  - IPv4: `169.254.0.0/16`.

---

## **IP Address Classes (IPv4)**

| Class | Range               | Purpose                                   |
|-------|---------------------|-------------------------------------------|
| A     | 0.0.0.0 - 127.255.255.255 | Used by large organizations like schools or universities for extensive networking needs. |
| B     | 128.0.0.0 - 191.255.255.255 | Suitable for mid-sized organizations like military or government bodies. |
| C     | 192.0.0.0 - 223.255.255.255 | Ideal for small businesses or home networks. |
| D     | 224.0.0.0 - 239.255.255.255 | Reserved for multicast communication, commonly used in streaming or conferencing. |
| E     | 240.0.0.0 - 255.255.255.255 | Reserved for experimental or research purposes. |

---

### 4. **Subnetting**:
- Divides an IP network into smaller segments to improve management and efficiency.
- Subnet mask: Defines network and host portions of an IP (e.g., `255.255.255.0` for `/24`).
- Calculating subnets -- determine class and then according to default subnet take host bits(n) , 2<sup>n</sup> and remaining host bits(m), 2<sup>m-2</sup>.

---

## **Tools for IP Address Management and Testing**

### **Command-Line Tools**:
- `ping`: Test connectivity to another device.
- `ipconfig`/`ifconfig`: View IP configuration.
- `traceroute`: Trace the path to a destination.
- `nslookup`: Resolve domain names to IPs.
- `netstat`: View active connections.


---
