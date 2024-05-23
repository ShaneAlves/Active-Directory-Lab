# Active-Directory-Lab
## Descrition
In this step-by-step guide, I went through the process of setting up a laboratory environment for Active Directory using Oracle VirtualBox. By configuring and running this lab, I was able to gain a deeper understanding of how Active Directory and Windows networking operates.
## Languages and Utilities Used
#### • PowerShell
## Environments Used 
#### • Windows 10 (21H2)
#### • Server 2019
# Lab Overview:
This is the guide I will be goinhg by:![image](https://github.com/ShaneAlves/Active-Directory-Lab/assets/111554296/7dff8ebd-e2cc-480a-93e3-5bf5754c0b05)

1. I downloaded Oracle VM to host my virtual machines. I had two different operating machines within Oracle (Windows 10 ISO and Windows Server 2019 ISO)

2. The first VM I created was the Domain Controller, which housed the Active Directory. This VM had two network adapters, one for the outside internet and the other for my VirtualBox private network.

3. After installation, I connected that VM to Server 2019 and assigned its IP addresses for my internal network; the external network got an automatic IP address from my home network.

4. Once step 3 was finished, I got the server set up, configured, and named (Domain Controller); I downloaded and installed Active Directory and created a domain for it.

5. After finishing that, I configured NAT and routing so the clients on the private network could reach the internet through the domain controller. In the last step in the Server 2019 VM, I set up a DHCP on the Domain Controller, so when I create my Windows 10 Machine, it can automatically get an IP address.

6. The last thing to do on the Domain Machine is to run a Powershell Strip that automatically creates users in Active Directory

7. After completing all that, I created my Client VM and installed Windows 10; this VM would be connected to the private virtual box network. I named the VM Client 1, attached it to the domain, and tested it all out by logging in to the VM using one of the users I created running my Powershell Script.
