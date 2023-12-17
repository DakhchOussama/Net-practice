# NetPractice Project

## Overview

**NetPractice** is an educational project aimed at providing a practical understanding of networking concepts. It covers fundamental topics such as IP addressing, subnetting, network masking, routing, and the role of devices like switches and routers in a network.

## Project Content

## 🌐 IP Address

An IP address is a unique identifier for a device on the internet or a local network. It stands for "Internet Protocol" and serves as a set of rules governing data format and transmission over networks.

In essence, IP addresses facilitate information exchange between devices by providing location information. They are expressed as a set of four numbers, such as 192.158.1.38, with each number ranging from 0 to 255.

### How IP Addresses Work

1. Your device connects to the internet indirectly through a network, such as your Internet Service Provider (ISP) at home or your company network at work.
2. The ISP assigns your device an IP address.
3. Internet activity goes through the ISP, which routes it back to your device using the assigned IP address.
4. Your IP address can change due to factors like turning your modem or router on/off.
5. When traveling, your device uses a different (temporary) IP address assigned by the ISP of the current network.

**IP Address Structure:**

- Octet 1 . Octet 2 . Octet 3 . Octet 4
- 1 Octet = 8 bits (xxxxxxxx . xxxxxxxx . xxxxxxxx . xxxxxxxx)
- Each bit (x) can be 0 or 1.

**Classes:**

- Class A: 0.0.0.0 to 127.255.255.255
- Class B: 128.0.0.0 to 191.255.255.255
- Class C: 192.0.0.0 to 223.255.255.255
- Class D: 224.0.0.0 to 239.255.255.255

**Network Masking:**

- The network mask distinguishes the network and host portions of an IP address.
- Common mask: 255.255.255.0 (street analogy).

**Subnet Mask: /30**

- Defines the range of IP addresses within a network or subnet.
- Example: 11111111.11111111.11111111.11111100 (32 bits).

**Routing Table:**

## 🔄 Switch

A switch connects multiple devices within a single network, distributing packets locally. It lacks interfaces to communicate outside its network.

## 🌐 Router

A router connects multiple networks, with an interface for each connected network. IP address ranges on router interfaces must not overlap.

### 📜 Public vs. Private Addresses

- **Public Address:** Assigned by the ISP, accessible over the internet.
- **Private Address:** Assigned by the router within a network (e.g., 192.168.x.x).

### 📌 Reserved Private IP Address Ranges

1. 192.168.0.0 – 192.168.255.255 (65,536 addresses)
2. 172.16.0.0 – 172.31.255.255 (1,048,576 addresses)
3. 10.0.0.0 – 10.255.255.255 (16,777,216 addresses)

If you want more informations, send your email Notion to my Email:

📧 oussamadakhch1999@gmail.com
