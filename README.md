<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark and experiment with Network Security Groups. <br />



## **What are NSGs?** ##
Network Security Groups (NSGs) in Azure are critical components for managing and controlling network traffic to and from Azure resources, such as virtual machines (VMs).
NSGs are firewall-like configurations in Azure that allow or deny inbound and outbound traffic to Azure resources at the network interface or subnet level.
They contain security rules that specify:
- **Source**: The origin of the traffic (IP address, range, or service tag).
- **Destination**: The target of the traffic (IP address, range, or service tag).
- **Port**: The port number or range of ports.
- **Protocol**: TCP, UDP, or any.
- **Action**: Allow or deny traffic.

Here's a breakdown of their role in inspecting traffic between Azure VMs:
<h2>Video Demonstration</h2>

- ### [YouTube: Azure Virtual Machines, Wireshark, and Network Security Groups](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04

<h2>High-Level Steps</h2>

Here are some high-level steps involved in configuring Network Security Groups (NSGs) and inspecting traffic between Azure Virtual Machines:

**Step 1: Create or Select NSGs:**

- If you don't have existing NSGs, create them.
- Associate the NSGs with the appropriate subnets or network interfaces of your virtual machines. An NSG can be associated with a subnet or with a single NIC.

**Step 2: Define Inbound and Outbound Rules:**

- Inbound Rules: Control traffic entering the virtual machine. Define rules that allow or deny traffic based on source IP addresses, ports, protocols (TCP, UDP, ICMP), and other criteria.
- Outbound Rules: Control traffic leaving the virtual machine. Define rules that allow or deny traffic based on destination IP addresses, ports, protocols, and other criteria.

**Step 3: Inspect Traffic Flow:**

- Analyze Network Security Group Logs: Monitor the NSG logs to track traffic flow and identify any security incidents or anomalies.
- Use Azure Monitor: Utilize Azure Monitor to collect and analyze network traffic data, including NSG logs, for deeper insights and security monitoring.
- Test Connectivity: Verify that the defined rules allow the expected traffic flow between your virtual machines.

**Step 4: Optimize and Refine Rules:**

- Review and update your NSG rules based on evolving security requirements and application needs.
- Principle of Least Privilege: Follow the principle of least privilege, granting only the necessary permissions to each virtual machine.
- Security Best Practices: Implement security best practices, such as using deny-by-default rules and regularly reviewing and updating your security configurations.

**Additional Considerations:**

- Virtual Network Peering: If you need communication between virtual machines in different subnets or virtual networks, configure virtual network peering and adjust NSG rules accordingly.
- Azure Firewall: Consider using Azure Firewall for more advanced security features, such as threat intelligence-based filtering and web application firewall (WAF).

Following these steps and adhering to security best practices, you can effectively secure traffic flow between your Azure Virtual Machines using Network Security Groups.

<h2>Actions and Observations</h2>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
