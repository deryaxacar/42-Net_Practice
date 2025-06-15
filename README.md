<h1 align="center">42 - Net_Practice 🌐</h1>

<!-- Project Logo or Image -->
<p align="center">
  <a target="blank"><img src="https://github.com/deryaxacar/42-Net_Practice/blob/main/netpractice.png" height="150" width="150" /></a>
</p>

<!-- Project Description -->
<p align="center">
  Net_Practice is a project developed as part of the 42 Network Bootcamp, designed to understand network programming and network protocols. This project comprehensively covers fundamental topics such as network configurations, communication protocols, and data encapsulation. Net_Practice enables users to develop network applications and evaluate the performance of existing networks. Offering both theoretical knowledge and practical experience, this project provides an in-depth look at network technologies.
</p>

---

### Table of Contents 🔗

- [Binary Number System](#binary-number-system)
   - [Table](#table)
   - [Explanation](#explanation)
- [IP Addresses: IPv4 and IPv6](#ip-addresses-ipv4-and-ipv6)
   - [IPv4 and IPv6 Formats](#ipv4-and-ipv6-formats)
   - [IPv4 vs IPv6 Comparison](#ipv4-vs-ipv6-comparison)
- [IP Address Classes](#ip-address-classes)
   - [Class A IP Address](#class-a-ip-address)
   - [Class B IP Address](#class-b-ip-address)
   - [Class C IP Address](#class-c-ip-address)
   - [Class D IP Address](#class-d-ip-address)
   - [Class E IP Address](#class-e-ip-address)
- [IP Address Classes and Calculations](#ip-address-classes-and-calculations)
- [IP Calculations](#ip-calculations)
   - [Subnet Calculation](#subnet-calculation)
   - [Subnet Mask](#subnet-mask)
   - [CIDR Notation](#cidr-notation)
   - [Usable IP Count Calculation](#usable-ip-count-calculation)
   - [Wildcard Mask](#wildcard-mask)
- [Example Calculations](#example-calculations)

---

![img](https://github.com/deryaxacar/42-Net_Practice/blob/main/ipsubnetting.png)

---

<h2 id="binary-number-system" align="center">Binary Number System</h2>

This table shows the bits in the binary number system along with their binary values, exponential powers, and decimal equivalents.

---

<div align="center" id="table">
  <table>
    <tr>
      <th>Bit</th>
      <th>Binary</th>
      <th>Exponential</th>
      <th>Decimal</th>
      <th>Bit</th>
      <th>Binary</th>
      <th>Exponential</th>
      <th>Decimal</th>
    </tr>
    <tr>
      <td>0</td>
      <td>0000</td>
      <td>2^0</td>
      <td>0</td>
      <td>6</td>
      <td>0110</td>
      <td>2^2 + 2^1</td>
      <td>6</td>
    </tr>
    <tr>
      <td>1</td>
      <td>0001</td>
      <td>2^0</td>
      <td>1</td>
      <td>7</td>
      <td>0111</td>
      <td>2^2 + 2^1 + 2^0</td>
      <td>7</td>
    </tr>
    <tr>
      <td>2</td>
      <td>0010</td>
      <td>2^1</td>
      <td>2</td>
      <td>8</td>
      <td>1000</td>
      <td>2^3</td>
      <td>8</td>
    </tr>
    <tr>
      <td>3</td>
      <td>0011</td>
      <td>2^1 + 2^0</td>
      <td>3</td>
      <td>9</td>
      <td>1001</td>
      <td>2^3 + 2^0</td>
      <td>9</td>
    </tr>
    <tr>
      <td>4</td>
      <td>0100</td>
      <td>2^2</td>
      <td>4</td>
      <td>10</td>
      <td>1010</td>
      <td>2^3 + 2^1</td>
      <td>10</td>
    </tr>
    <tr>
      <td>5</td>
      <td>0101</td>
      <td>2^2 + 2^0</td>
      <td>5</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
  </table>
</div>

---

#### Explanation

The binary number system uses only two digits: 0 and 1. Each bit represents a power of 2. The table shows the binary representations of decimal numbers from 0 to 10, how each bit corresponds to powers of 2, and their equivalent values in the decimal system.

- **Bit**: The number in the decimal system.
- **Binary**: The binary representation of each decimal number.
- **Exponential**: The value of each bit expressed as a power of 2.
- **Decimal**: The decimal equivalent of the binary value.

For example, the decimal number 5 is written as 0101 in binary. This is calculated as 2^2 + 2^0 (4 + 1), which equals 5 in the decimal system. This system is widely used in digital electronics and computer science.

---

## <div align="center">IP Addresses: IPv4 and IPv6</div>

IPv6 was developed to overcome the limitations of IPv4 and to meet the growing demands of the internet. With the increasing use of applications like IoT (Internet of Things), the importance of IPv6 has become even more evident.

---

#### <div align="center">IPv4 and IPv6 Formats</div>

| Feature                | IPv4                                        | IPv6                                                   |
|------------------------|---------------------------------------------|--------------------------------------------------------|
| **Address Length**     | 32 bits                                     | 128 bits                                               |
| **Address Structure**  | Four octets, values between 0–255           | Eight groups, four-digit hexadecimal (0–FFFF)          |
| **Notation**           | Dotted-decimal notation                     | Eight groups separated by colons (:)                   |
| **Example Address**    | 192.168.0.1                                  | 2001:0db8:85a3:0000:0000:8a2e:0370:7334                |

---

#### <div align="center">IPv4 vs IPv6 Comparison</div>

| Feature                 | IPv4                                        | IPv6                                        |
|-------------------------|---------------------------------------------|---------------------------------------------|
| **Address Length**      | 32 bits                                     | 128 bits                                    |
| **Address Format**      | Four octets (0–255), separated by dots      | Eight groups, hexadecimal, separated by colons (:) |
| **Example Address**     | 192.168.0.1                                  | 2001:0db8:85a3:0000:0000:8a2e:0370:7334      |
| **Address Capacity**    | Approximately 4.3 billion addresses         | 340 undecillion (3.4 x 10^38) addresses      |
| **Representation**      | Decimal                                     | Hexadecimal                                  |
| **Address Exhaustion**  | Limited and depleted                        | Vast space, no exhaustion issue              |
| **Header Structure**    | Simpler, contains less information          | More complex, optimized for performance      |
| **Auto-Configuration**  | DHCP                                        | SLAAC and DHCPv6                             |

---

### <div align="center">IP Address Classes</div>

This table shows the classes of IP addresses and their respective characteristics.

| Class | Start Address    | End Address      | Subnet Mask           | Number of Networks | Max Hosts per Network | Use Case               |
|-------|------------------|------------------|------------------------|--------------------|------------------------|------------------------|
| A     | 0.0.0.0          | 127.255.255.255  | 255.0.0.0 (/8)         | 128                | 16,777,214             | Large networks         |
| B     | 128.0.0.0        | 191.255.255.255  | 255.255.0.0 (/16)      | 16,384             | 65,534                 | Medium-sized networks  |
| C     | 192.0.0.0        | 223.255.255.255  | 255.255.255.0 (/24)    | 2,097,152          | 254                    | Small networks         |
| D     | 224.0.0.0        | 239.255.255.255  | Not used               | Not applicable     | Not applicable         | Multicast              |
| E     | 240.0.0.0        | 255.255.255.255  | Not used               | Not applicable     | Not applicable         | Experimental, research |

IP addresses are categorized into classes to better manage networks. These classes differ based on the size and purpose of the network. Classes A, B, and C are suitable for different network scales, while Class D is used for multicast, and Class E is reserved for experimental use.

### Explanation:

- #### Class A IP Address
  - Used for large networks. The first octet (0–127) represents the network portion.
  - **Example Address:** 10.0.0.1
  - **Explanation:** 10.0.0.1 is a Class A IP address. Class A is used in large networks with a wide range of addresses. The first octet (10) represents the network part, while the remaining three (0.0.1) are for host identification.
  - **Usable Range:** 1.0.0.0 – 126.255.255.255

- #### Class B IP Address
  - Used for medium-sized networks. The first two octets (128–191) identify the network.
  - **Example Address:** 172.16.0.1
  - **Explanation:** 172.16.0.1 is a Class B IP address. Class B is designed for medium-sized networks. The first two octets (172.16) are the network portion, and the remaining two (0.1) are for the host.
  - **Usable Range:** 128.0.0.0 – 191.255.255.255

- #### Class C IP Address
  - Used for small networks. The first three octets (192–223) define the network.
  - **Example Address:** 192.168.1.1
  - **Explanation:** 192.168.1.1 is a Class C IP address. Class C is intended for small networks. The first three octets (192.168.1) define the network, and the last octet (1) is used for the host.
  - **Usable Range:** 192.0.0.0 – 223.255.255.255

- #### Class D IP Address
  - Used for multicast addressing. Not used for standard network addressing.
  - **Example Address:** 224.0.0.1
  - **Explanation:** 224.0.0.1 is a Class D IP address. Class D is used in multicast communication, allowing data transmission to specific groups of devices on a network.
  - **Range:** 224.0.0.0 – 239.255.255.255

- #### Class E IP Address
  - Reserved for experimental purposes. Not used in standard network addressing.
  - **Example Address:** 240.0.0.1
  - **Explanation:** 240.0.0.1 is a Class E IP address. These addresses are used for research and experimental purposes and are not intended for general use in public networks.
  - **Range:** 240.0.0.0 – 255.255.255.255

---

### <div align="center">IP Address Classes and Calculations</div>

IP addresses are classified based on the size and usage of networks. Each class has different address ranges, subnet masks, and calculation methods.

| Class | Start Address     | End Address       | Subnet Mask           | Number of Networks | Max Hosts per Network  | Use Case               |
|-------|-------------------|-------------------|------------------------|--------------------|-------------------------|------------------------|
| A     | 0.0.0.0           | 127.255.255.255   | 255.0.0.0 (/8)         | 128                | 16,777,214              | Large networks         |
| B     | 128.0.0.0         | 191.255.255.255   | 255.255.0.0 (/16)      | 16,384             | 65,534                  | Medium-sized networks  |
| C     | 192.0.0.0         | 223.255.255.255   | 255.255.255.0 (/24)    | 2,097,152          | 254                     | Small networks         |
| D     | 224.0.0.0         | 239.255.255.255   | Not used               | Not applicable     | Not applicable          | Multicast              |
| E     | 240.0.0.0         | 255.255.255.255   | Not used               | Not applicable     | Not applicable          | Experimental, research |

---

### <div align="center">IP Calculations</div>

#### **Subnet Calculation**
Subnets are used to divide a block of IP addresses into smaller networks. When subnetting, the network ID and host ID are defined.

**Example:**  
If a network uses the 192.168.1.0/24 IP block:
- Subnet Mask: 255.255.255.0  
- First IP Address (Network ID): 192.168.1.0  
- Last IP Address (Broadcast): 192.168.1.255  
- Usable IP Range: 192.168.1.1 - 192.168.1.254 (Total of 254 hosts)

#### **Subnet Mask**
A subnet mask is used to distinguish the network and host portions of an IP address. CIDR notation (e.g., /24, /16) represents this mask.

**Example:**
- **/24** Subnet Mask: 255.255.255.0  
- **/16** Subnet Mask: 255.255.0.0

#### **CIDR Notation**
CIDR (Classless Inter-Domain Routing) allows for more flexible representation of IP addresses and subnets.

**Example:**  
192.168.1.0/24 represents 256 IP addresses and has a subnet mask of 255.255.255.0.

#### **Usable IP Count Calculation**
The number of usable IP addresses in a subnet is calculated with the formula:  
`Usable IPs = 2^(32 - CIDR) - 2`

**Example:**
- For /24: 2^(32 - 24) - 2 = 256 - 2 = 254 usable IPs  
- For /16: 2^(32 - 16) - 2 = 65,536 - 2 = 65,534 usable IPs

#### **Wildcard Mask**
A wildcard mask is the inverse of a subnet mask and is often used in ACLs (Access Control Lists) and other security configurations.

**Example:**
- For subnet mask 255.255.255.0, the wildcard mask is: 0.0.0.255

---

### Example Calculations

**Network:** 192.168.1.0/24  
- Subnet Mask: 255.255.255.0  
- CIDR Notation: /24  
- Usable IP Range: 192.168.1.1 - 192.168.1.254  
- Broadcast Address: 192.168.1.255  
- Total Hosts: 254

**Network:** 10.0.0.0/8  
- Subnet Mask: 255.0.0.0  
- CIDR Notation: /8  
- Usable IP Range: 10.0.0.1 - 10.255.255.254  
- Broadcast Address: 10.255.255.255  
- Total Hosts: 16,777,214

---

<p align="center">2025 This project was created by Derya ACAR.</p>
