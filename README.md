# Network Traffic Analysis with Wireshark

## Overview
This project demonstrates the use of Wireshark, a powerful network packet analyzer, to capture and analyze various types of network traffic within a virtual network environment hosted on Azure. The focus is on understanding network behavior through protocols such as ICMP, SSH, DHCP, DNS, and RDP.

## Environments and Technologies Used
- **Wireshark**: Network protocol analyzer
- **Microsoft Azure**: Virtual Machines for Windows 10 and Ubuntu
- **Operating Systems Used**:
  - Windows 10 (for capturing traffic)
  - Ubuntu (as a secondary system to generate network activities)

## High-Level Analysis Steps
1. **Setup Virtual Machines in Azure**:
   - Configure VMs within a resource group and virtual network to simulate network interactions.
2. **Install and Configure Wireshark**:
   - Prepare Wireshark on the Windows 10 VM to capture network traffic.
3. **Capture and Analyze Network Traffic**:
   - Conduct detailed traffic analysis across multiple protocols to diagnose behaviors and security implications.

## Detailed Analysis and Configuration Steps

### Step 1: Setup Virtual Machines in Azure
- **Create Resource Group and Virtual Network**:
  - Establish a resource group and a virtual network in Azure, adding both Windows 10 and Ubuntu VMs to simulate a mixed network environment.
  - Azure dashboard showing the resource group, VMs, and network configurations:
    ![image](https://github.com/00chazz/wireshark-analysis/assets/63687898/ce75a80b-3b1f-4f2b-8e75-18d7e1a4b252)


### Step 2: Install and Configure Wireshark
- **Installation on Windows 10 VM**:
  - Download and install Wireshark on the Windows 10 VM. Configure it to monitor the virtual network interface.
  - Once Wireshark is installed, we can monitor the traffic by pressing the blue button:
    ![image](https://github.com/00chazz/wireshark-analysis/assets/63687898/139ce3e8-cebd-4e07-8d94-762f373720f7)


### Step 3: Capture and Analyze Network Traffic
- **Observe ICMP Traffic**:
  - Capture ICMP traffic as you ping from Windows 10 to Ubuntu VM, and observe both request and reply packets. Manipulate Network Security Group settings to see changes in ICMP traffic visibility.
  - We can see Wireshark capturing ICMP traffic when we ping the Ubuntu Server's Private IP:
  ![image](https://github.com/00chazz/wireshark-analysis/assets/63687898/c269f931-3742-46ea-8e8f-52b98ea1e965)

- **Monitor SSH Traffic**:
  - Capture SSH traffic from the Windows VM to the Ubuntu VM, detailing the SSH handshake and session data.
    ![image](https://github.com/00chazz/wireshark-analysis/assets/63687898/913526fc-f5b3-4721-bcd0-f96b75eea927)


- **Track DHCP Traffic**:
  - Record DHCP traffic during a lease renewal process executed from the Windows VM.
  - ![image](https://github.com/00chazz/wireshark-analysis/assets/63687898/9f441525-3182-4d4f-a74d-2af8a747596e)


- **Analyze DNS Traffic**:
  - Capture DNS resolution traffic as the Windows VM performs nslookup operations for domains like google.com and disney.com.
    ![image](https://github.com/00chazz/wireshark-analysis/assets/63687898/1c9f35a5-20ab-4968-8634-9e49b98054e5)


- **Examine RDP Traffic**:
  - Observe and analyze RDP traffic between the Windows VM and another remote system to understand the continuous traffic flow typical for RDP sessions.
  - The flow is constant as the Remote Desktop is constantly being streamed to the host computer:
    ![image](https://github.com/00chazz/wireshark-analysis/assets/63687898/ad664b47-9975-44ae-b78a-853542a5e684)


## Conclusion
This project uses Wireshark to provide deep insights into the functionality and security of network protocols within a virtualized environment. By analyzing traffic patterns and responses, this setup enhances understanding of network security, efficiency, and operational challenges.

## Conclusion
Using Wireshark for network traffic analysis provides valuable insights into network operations, security vulnerabilities, and troubleshooting. This project showcases the utility of detailed packet analysis in understanding and securing network environments.

## Connect with Me
- **LinkedIn:** [Chazz Conino](https://www.linkedin.com/in/chazz-c-382a75122/)
