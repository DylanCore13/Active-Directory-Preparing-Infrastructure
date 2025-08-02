# Active-Directory: Preparing the Infrastructure

<img width="1536" height="1011" alt="image" src="https://github.com/user-attachments/assets/c86da1b0-e3d1-4be0-aa8d-6f5f573a57e3" />

<h2> Objective </h2>

- This setup guide outlines configuring an Azure-based Active Directory lab by first creating a resource group, virtual network, and a Windows Server 2022 VM named "DC-1" with a static private IP and disabled firewall. Subsequently, a Windows 10 VM named "Client-1" is provisioned within the same network, its DNS settings are configured to point to "DC-1"'s private IP, and connectivity is verified by pinging "DC-1" and checking the DNS settings via ipconfig /all on "Client-1".

<h2>Skills Used</h2>

- Azure Resource Management: Creating and managing resource groups, virtual machines (VMs), and virtual networks (VNets). This involves understanding how to provision and configure resources within the Azure cloud environment.

Networking Concepts: Setting up and configuring virtual networks, subnets, and managing IP addressing (specifically assigning static IP addresses). Understanding DNS resolution is also crucial for the client-server communication.

Windows Server Administration: Installing and configuring the Active Directory Domain Services (AD DS) role on a Windows Server VM, promoting it to a domain controller, and managing its DNS settings.

Client-Server Connectivity: Troubleshooting network connectivity (ping) and verifying network configurations (ipconfig /all) on a client machine.
