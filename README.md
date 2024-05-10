<h1>Two-VPCs-with-full-mesh-VPC-Peering-</h1>

<h2>Description</h2>
Implemented a robust and scalable dual-VPC network architecture on AWS, facilitating seamless communication between resources through full mesh VPC peering. This deployment included the configuration of EC2 instances within each VPC, comprising web servers and a bastion host, with stringent security measures to ensure secure SSH access and maintain infrastructure integrity. Network access controls, including NAT Gateway for outbound internet access and IPv6 enablement on public subnets, were implemented to enhance network capabilities and facilitate future scalability."
<br />
<br />
<br />
<h2>
<p align="center">
Main Diagram<br/>
 <br />
<img src="https://imgur.com/yG3CtVW.png" height="40%" width="80%" alt="Disk Sanitization Steps"/></p>
<br /></h2>
<br />
<h2>Languages and Utilities Used</h2>

- <b>AWS CloudFormation for infrastructure provisioning and management.</b>
- <b>Python with Boto3 library for scripting and automation of EC2 instance deployment and configuration.</b>
- <b>SSH for secure remote access to EC2 instances.</b>
- <b>IPv6 for network addressing and connectivity.</b>
- <b>NAT Gateway for outbound internet access from private subnets.</b>
- <b>Amazon VPC for creating and managing the dual-VPC network architecture.</b>
- <b>Bastion host for secure SSH access to the private resources within the VPCs.</b>

<h2>Environments Used </h2>

- <b>AWS Management Console for initial setup and configuration.</b>
- <b>Local development environment for scripting and testing Python automation scripts.</b>
- <b>AWS Command Line Interface (CLI) for command-line interactions with AWS services.</b>
- <b>Text editors or Integrated Development Environments (IDEs) for writing and editing Python scripts and CloudFormation templates.</b>

<h2>Program walk-through:</h2>

- <b>Network Topology Design:</b> Created a comprehensive network topology featuring two Virtual Private Clouds (VPCs) interconnected via full mesh VPC peering.
- <b>EC2 Instance Configuration:</b> Configured EC2 instances within each VPC, including web servers (web-dev, web-A, web-B) and a bastion host to facilitate secure SSH access.
- <b>Subnet Setup:</b> Established a new private subnet for the web-dev EC2 instance and ensured access to external resources via a NAT Gateway located in the public subnet.
- <b>SSH Access Configuration:</b> Configured SSH access for the account user to the bastion host, enabling SSH connectivity to the web-dev EC2 instance from the bastion host.
- <b>Inter-VPC Communication:</b> Enabled communication between web-A and web-B instances in VPC-A and VPC-B respectively, and the web-dev server in the default VPC, allowing access via curl to 
     the IPv4 address.
- <b>IPv6 Enablement:</b> Enabled IPv6 on public subnets in VPC-A and VPC-B to enhance network capabilities and support future scalability.
- <b>IPv4 Connectivity:</b> Configured EC2 instances web-A and web-B to communicate with each other using their IPv4 addresses, ensuring seamless connectivity within the network architecture.







<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
