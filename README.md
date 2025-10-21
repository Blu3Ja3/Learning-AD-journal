# Learning-AD-journal
This is my journey of creating and working in AD on my personal VM

Active Directory (AD) is a foundational technology used by the vast majority of large enterprises — often estimated at around 90%. I first encountered AD during my IT schooling and early professional experience, where I worked with user provisioning and deprovisioning.

At my next role, AD wasn’t part of the tech stack, and over time I lost hands-on exposure. Now, as I grow my cybersecurity skill set, I’m committed to relearning and deepening my knowledge of Active Directory — not just as a directory service, but as a key part of identity security and blue team operations.

### Day 1

Setting Up My Lab

I started by downloading Windows Server 2022 and creating a new virtual machine (VM) in VirtualBox.

VM settings:
Name: WinServer
Type: Microsoft Windows
Version: Windows Server 2022 (64-bit)

In the VM settings, under Storage, I selected the empty optical disk and mounted the Windows Server 2022 ISO. Once attached, I launched the VM to begin the installation.

### Choosing the Server Edition 

When prompted, I had four installation options:

Windows Server Standard Core
Windows Server Standard (Desktop Experience)
Windows Server Datacenter Core
Windows Server Datacenter (Desktop Experience)

I decided to install both Core and Desktop Experience versions — with the goal of eventually becoming more comfortable in the command line (Core), but for now, I focused on the Desktop Experience, which provides a GUI and is more familiar.

### Installing Active Directory Domain Services (AD DS) ##

After logging into my Windows Server, I opened Server Manager and followed these steps:

Go to Manage → Add Roles and Features
Select Role-based or feature-based installation
Choose the local server
On the Server Roles screen, select Active Directory Domain Services
Click Install

Once installation was complete, a yellow flag appeared in Server Manager. I clicked it to promote the server to a domain controller.

I chose:
Add a new forest
Domain name: JSlab.local
Kept default settings and completed the installation

The server restarted, and I was able to log into my new domain.

Once logged in, I opened Active Directory Users and Computers from the Tools menu in Server Manager.
I now have a fully functional AD lab environment!

### This is just the beginning. My upcoming goals include:

Creating and managing users, groups, and organizational units (OUs)
Exploring Group Policy Objects (GPOs)
Automating tasks with PowerShell
Practicing detection and response from a blue team perspective

Stay tuned — this is part of a larger journey to grow my skills in cybersecurity, and I’ll continue sharing my progress.

### Want to Follow Along?
I'll be documenting this homelab journey as I learn tools like PowerShell, Linux, Python, and SIEM/logging practices — all essential skills for a SOC analyst role.

Thanks for reading!
