<p align="center">
<img width="621" alt="Screen Shot 2023-07-15 at 11 07 25 AM" src="https://github.com/SiclaitGitHub/azure-sentiel/assets/139138443/729f7da7-d0d2-45b8-a6ea-71d4cea6cb98">


</p>

<h1> Azure Sentinel Installation</h1>
This tutorial outlines the prerequisites and installation of Azure Sentinel.<br />


<h2>Video Demonstration</h2>

- ### [SIEM Tutorial for Beginners | Azure Sentinel Tutorial MAP with LIVE CYBER ATTACKS](https://www.youtube.com/watch?v=RoZeVbbZ0o0)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Computer)
- Microsoft Remote Desktop
- Azure Sentinel (Microsoft)
- Log Analytics Workspace (Azure)
- PowerShell

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>High Level Steps</h2>

- Create Virtual Machine - VM1 (Azure)
- Configure VM1's Firewall (Azure)
- Connect VM1 to Microsoft Remote Desktop 
- 
- 

<h2>Installation Steps</h2>

<img width="908" alt="Screen Shot 2023-07-10 at 1 30 29 PM" src="https://github.com/SiclaitGitHub/osticket-prereqs/assets/139138443/4f97a83e-1c37-4210-9dc1-8530cb7f91bf">


1. Set up your Azure Virtual Machine (Windows 10)

Azure is a cloud computing platform and service offered by Microsoft. It provides a wide range of cloud services that enable organizations to build, deploy, and manage applications and services through Microsoft-managed data centers.

A virtual machine (VM) on Microsoft Azure is a computing resource that uses software instead of a physical computer to run programs and deploy apps. Each VM instance can run its own operating system (OS), which means multiple VMs can run different operating systems on the same physical machine.

Create a new Azure resource group, virtual network, subnet and virtual machine running Windows 10. Choose a VM size according to your needs. Once the VM is set up, you will need to connect to it using Remote Desktop. For this, you'll need the public IP address of the VM and the credentials you provided during the VM setup.
</p>
<br />


<img width="1432" alt="Screen Shot 2023-07-16 at 12 36 27 PM" src="https://github.com/SiclaitGitHub/azure-sentiel/assets/139138443/c3cabe72-89ab-44b1-a50a-8a09e34b4ad0">

2. Configure Firewall in "Network" Settings when creating VM1 in Azure.

- Under the "Networking" tab in the VM1 creation window
- Select "Advanced" for the Network Security Group Option
- Then Click "Create New"
- Remove the default "Inbound Rule" then select "Add Inbound Rule"
- Type "*" for the "Destination Port" option.
- Select "Any" for the "Protocol"


<img width="856" alt="Screen Shot 2023-07-19 at 6 51 27 PM" src="https://github.com/SiclaitGitHub/azure-sentiel/assets/139138443/c4f13910-adcd-49ec-9a01-4de67073efe0">

3. Create Log Alanytics Workspace (LAW) in Azure

- Type "Log Alanytics Workspace" in the search bar of the Azure window
- Make sure the LAW is set to the same 'Resource Group" and "Region" as VM1
- Click "Review + Create"
- Click Create


<img width="602" alt="Screen Shot 2023-07-15 at 11 22 30 AM" src="https://github.com/SiclaitGitHub/azure-sentiel/assets/139138443/63021c1d-022d-4f60-972d-854648a0586e">

2. Connect VM1 to Microsoft Remote Desktop

SIEM stands for Security Information and Event Management. It refers to a category of software solutions and technologies that help organizations collect, analyze, and manage security event and log data from various sources across their network infrastructure.

The primary purpose of SIEM is to provide organizations with a centralized platform for real-time monitoring, detection, and response to security incidents and threats. SIEM solutions collect data from a wide range of sources, including security devices (such as firewalls, intrusion detection systems, and antivirus software), servers, applications, and network infrastructure. This data is then aggregated, correlated, and analyzed to identify patterns, anomalies, and potential security breaches.

 - Open Microsoft Remote Desktop on your local computer
 - Enter the Public IP Address of VM1
 - Enter login credentials created in Azure when setting up VM1
 - Virtual Desktop should appear upon log in.
   

<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

2. Install Azure Sentinel
   
Azure Sentinel is a cloud-native security information and event management (SIEM) and security orchestration automated response (SOAR) solution provided by Microsoft. It is a part of the Microsoft Azure cloud platform and is designed to help organizations detect, investigate, and respond to security threats and incidents across their entire environment.

Azure Sentinel collects and analyzes security event data from various sources, including logs from on-premises systems, cloud services, security devices, and third-party products. It uses advanced analytics, machine learning, and artificial intelligence capabilities to detect anomalies, identify threats, and provide intelligent security insights.

SIEM stands for Security Information and Event Management. It refers to a category of software solutions and technologies that help organizations collect, analyze, and manage security event and log data from various sources across their network infrastructure.

The primary purpose of SIEM is to provide organizations with a centralized platform for real-time monitoring, detection, and response to security incidents and threats. SIEM solutions collect data from a wide range of sources, including security devices (such as firewalls, intrusion detection systems, and antivirus software), servers, applications, and network infrastructure. This data is then aggregated, correlated, and analyzed to identify patterns, anomalies, and potential security breaches.




