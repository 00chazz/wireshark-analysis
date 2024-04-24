# Network Traffic Analysis with Wireshark

## Overview
This project demonstrates the use of Wireshark, a powerful network packet analyzer, to capture and analyze various types of network traffic. The aim is to understand network behavior, troubleshoot network problems, and gain insights into network security and performance based on real traffic scenarios.

## Environments and Technologies Used
- **Wireshark**: Network protocol analyzer
- **Operating Systems Used**:
  - Windows 10
- **Network Protocols Analyzed**:
  - ICMP (Internet Control Message Protocol)
  - SSH (Secure Shell)
  - DHCP (Dynamic Host Configuration Protocol)
  - DNS (Domain Name System)
  - RDP (Remote Desktop Protocol)

## High-Level Analysis Steps
1. **Setup Wireshark on Windows 10**:
   - Install Wireshark and configure it to capture traffic on a designated network interface.
2. **Capture Network Traffic**:
   - Perform captures for different types of network traffic, including ICMP, SSH, DHCP, DNS, and RDP.
3. **Analyze Captured Traffic**:
   - Examine the details of each protocol's operation and behavior under various conditions.

## Detailed Analysis and Configuration Steps

### Step 1: Setup Wireshark
- **Installation**:
  - Download and install Wireshark from the official website on a Windows 10 machine.
  - **Screenshot**: Show the successful completion of the Wireshark installation.

- **Configure Network Interface for Capture**:
  - Select the appropriate network interface for traffic capture in Wireshark.
  - **Screenshot**: Display the Wireshark interface selection screen.

### Step 2: Capture and Analyze Network Traffic
- **Capture ICMP Traffic**:
  - Use Wireshark to capture ICMP traffic while pinging known IPs both within and outside the network.
  - **Screenshot**: Capture the Wireshark screen showing ICMP traffic details, including request and reply packets.

- **Capture SSH Traffic**:
  - Record SSH session traffic by logging into a remote server via SSH while Wireshark is running.
  - **Screenshot**: Display SSH packets, highlighting the handshake and data encryption stages.

- **Capture DHCP Traffic**:
  - Observe the DHCP lease process by releasing and renewing an IP address on a client machine.
  - **Screenshot**: Show DHCP DISCOVER, OFFER, REQUEST, and ACK packets in Wireshark.

- **Capture DNS Traffic**:
  - Analyze DNS resolution traffic by using `nslookup` for various domain names.
  - **Screenshot**: Illustrate DNS query and response packets in Wireshark.

- **Capture RDP Traffic**:
  - Monitor traffic during a Remote Desktop session to observe the continuous data flow.
  - **Screenshot**: Highlight RDP packets showcasing the session initiation and data transmission.

### Step 3: Document Findings and Conclusions
- **Analysis Summary**:
  - Discuss the implications of the observed traffic patterns, particularly focusing on security and network efficiency.
  - **Screenshot**: Optional, include graphs or tables summarizing the traffic analysis.

## Conclusion
Using Wireshark for network traffic analysis provides valuable insights into network operations, security vulnerabilities, and troubleshooting. This project showcases the utility of detailed packet analysis in understanding and securing network environments.

## Connect with Me
- **LinkedIn:** [Chazz Conino](https://www.linkedin.com/in/chazz-c-382a75122/)
