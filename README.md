# Active-Directory: Preparing the Infrastructure

<img width="1536" height="1011" alt="image" src="https://github.com/user-attachments/assets/c86da1b0-e3d1-4be0-aa8d-6f5f573a57e3" />

<h2> Objective </h2>

- This setup guide outlines configuring an Azure-based Active Directory lab by first creating a resource group, virtual network, and a Windows Server 2022 VM named "DC-1" with a static private IP and disabled firewall. Subsequently, a Windows 10 VM named "Client-1" is provisioned within the same network, its DNS settings are configured to point to "DC-1"'s private IP, and connectivity is verified by pinging "DC-1" and checking the DNS settings via ipconfig /all on "Client-1".

<h2>Skills Used</h2>

- Azure Resource Management: Creating and managing resource groups, virtual machines (VMs), and virtual networks (VNets). This involves understanding how to provision and configure resources within the Azure cloud environment.

- Networking Concepts: Setting up and configuring virtual networks, subnets, and managing IP addressing (specifically assigning static IP addresses). Understanding DNS resolution is also crucial for the client-server communication.

- Windows Server Administration: Installing and configuring the Active Directory Domain Services (AD DS) role on a Windows Server VM, promoting it to a domain controller, and managing its DNS settings.

- Client-Server Connectivity: Troubleshooting network connectivity (ping) and verifying network configurations (ipconfig /all) on a client machine.


<h2>Services Used</h2>

- Azure Virtual Machines (VMs): Used to host both the Windows Server 2022 (DC-1) and Windows 10 (Client-1) operating systems.

- Azure Virtual Network (VNet): Provides the isolated and secure network environment for the VMs to communicate.

- Azure Subnets: Logical divisions within the VNet to organize and isolate resources.

- Azure Network Interface Cards (NICs): Components attached to VMs that enable network connectivity, and where static IP addresses are configured.



<b>


You'll first start off by creating a resource group and naming it Active-Directory-Lab, and make sure it's in the region US East 2


<img width="1066" height="477" alt="image" src="https://github.com/user-attachments/assets/5542ed4a-5018-4403-b161-241c3c3d2ce5" />




</b>


After that we'll create the Virtual Network, naming it Active-Directory-VNet and making sure it's in the Active-Directory-Lab resource group and same region (US East 2)

<img width="1006" height="492" alt="image" src="https://github.com/user-attachments/assets/4698192b-65b3-4ea1-a12a-13af1aa62d71" />



For your Virtual Machine, make sure its in the resource group "Active-Directory-Lab", name this VM "DC-1"

<img width="976" height="532" alt="image" src="https://github.com/user-attachments/assets/f7fc7087-1974-48a4-b70c-e29926541148" />



<img width="871" height="473" alt="image" src="https://github.com/user-attachments/assets/4f03421f-f93f-4661-af3f-7803c5b252dc" />


<img width="849" height="410" alt="image" src="https://github.com/user-attachments/assets/eec49f6e-a67e-4389-93f5-d01ec365f8ba" />



<img width="857" height="487" alt="image" src="https://github.com/user-attachments/assets/06dd03cb-f74b-461e-947e-2bd75bfe3a34" />




<img width="808" height="382" alt="image" src="https://github.com/user-attachments/assets/d54a9ccd-9ea6-47f9-970b-d4acb800e185" />



<img width="1162" height="462" alt="image" src="https://github.com/user-attachments/assets/28061116-00a4-4943-bb48-ea679b45ca6c" />




<img width="1314" height="532" alt="image" src="https://github.com/user-attachments/assets/907d50a9-b884-42ad-8b38-57ea7fde71a5" />



<img width="1188" height="454" alt="image" src="https://github.com/user-attachments/assets/f47c39cd-08af-42ad-baa6-fe62f89f91ab" />





<img width="1211" height="578" alt="image" src="https://github.com/user-attachments/assets/692e92ef-de44-4b69-b8e1-a48a14a35ebc" />


<img width="1088" height="480" alt="image" src="https://github.com/user-attachments/assets/e862479f-b198-46dc-a679-4c682bd6dc5f" />

<img width="1139" height="501" alt="image" src="https://github.com/user-attachments/assets/8d772da3-ca16-4913-babf-b212c6d5b8c5" />


<img width="846" height="476" alt="image" src="https://github.com/user-attachments/assets/8d8937d3-44b9-42a1-b6e1-8c4861f133c9" />


<img width="1239" height="593" alt="image" src="https://github.com/user-attachments/assets/a6823ec8-3778-43d7-bece-5191902d21aa" />


<img width="975" height="526" alt="image" src="https://github.com/user-attachments/assets/ccbfb4b5-b8af-4b9d-9475-8d7b9cf9d85a" />



