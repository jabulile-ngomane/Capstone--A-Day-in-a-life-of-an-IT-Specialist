# Capstone--A-Day-in-a-life-of-an-IT-Specialist
## OVERVIEW

This report documents the setup, configuration, and support activities performed in a small business IT environment. The aim was to showcase practical abilities in system installation, networking, server setup, security assessment, and problem-solving.
All activities were conducted in a regulated setting utilizing a Windows system and a virtualized Linux server. The project demonstrates actual IT support duties like user onboarding, ensuring network connectivity, system security, and troubleshooting technical problems.

## USER & SYSTEM CONFIGURATION
During the onboarding process for new users in the organization, local user accounts and security groups were established with PowerShell to replicate enterprise-level user and access management practices.
### Tasks Performed:
•	Created local user account:
net user intern2 Password123 /add & IT-Admin
•	Created security group:
net localgroup supportteam /add
•	Added user to group:
net localgroup supportteam intern2 /add
•	Verified user configuration:
net user intern2
<img width="620" height="421" alt="image" src="https://github.com/user-attachments/assets/a8d8e590-7a88-4e5a-b21d-664f5429fdfb" />

 <img width="756" height="399" alt="image" src="https://github.com/user-attachments/assets/9bf92185-04e9-4dbd-b345-38830bf9e170" />

 
### Key Concepts Demonstrated:
•	Role-Based Access Control (RBAC)
•	Principle of Least Privilege
•	Local account and group management
•	Command-line administration
### Software Deployment
The Windows operating system was already installed on my PC, and I installed the application software using Chocolatey.
Installed VLC using Chocolatey:
•	Installed Git using Chocolatey:
choco install vlc -y
 
<img width="608" height="355" alt="image" src="https://github.com/user-attachments/assets/9f05e30c-66c7-48b3-8973-cf6edc9d9a42" />


### Verified installation:
Choco list vlc
 <img width="628" height="323" alt="image" src="https://github.com/user-attachments/assets/b80f8834-54bd-4ced-b180-4d1c0d5caef9" />

This illustrates automated software installation and package management within a Windows setting.
### Outcome:
•	User accounts successfully created 
•	Permissions correctly applied

## NETWORK CONFIGURATION
To facilitate effective communication within the organization, network configuration and connectivity tests were conducted using command-line tools.
### IP Configuration:
Command used:
•	ipconfig /all
•	Ping default 172.20.6.1
•	Ping google.com
•	Ping 8.8.8.8
•	Ping to another PC
Results:
•	0% packet loss observed
•	Successful LAN and internet connectivity
•	DNS resolution is functioning correctly 

<img width="519" height="311" alt="image" src="https://github.com/user-attachments/assets/ec15f652-fe76-4342-870f-978727030245" />

### Outcome:
•	Valid IP configuration confirmed 
•	LAN connectivity verified 
•	Internet access confirmed 
•	DNS resolution is functioning correctly
4. SERVER AND INFRASTRUCTURE SERVICES (LINUX & WINDOWS)
To simulate real-world IT infrastructure, both Windows and Linux server environments were configured. This demonstrates cross-platform system administration skills commonly required in enterprise environments.
### Environment
•	OS: Windows 10
•	Virtualization: VirtualBox
•	Server OS: Ubuntu
•	Tools: PowerShell, Command Prompt, IIS, Apache
•	Network: Local LAN
#### Linux Server – Apache Web Server 
A Linux-based Apache web server was deployed using a virtual machine running Ubuntu.
#### Tools used:
•	Ubuntu Linux (Virtual Machine)
•	Apache Web Server
•	VirtualBox


#### Installation:
sudo apt update
sudo apt upgrade -y
sudo apt install apache2 -y
sudo systemctl status apache2
 <img width="628" height="282" alt="image" src="https://github.com/user-attachments/assets/d7aae49c-83d3-4740-90f1-e703b13c6ab8" />

Verification:
 <img width="573" height="288" alt="image" src="https://github.com/user-attachments/assets/c89d44a3-b5cf-4937-ac53-d271fd78f76e" />


Website Configuration:
 <img width="561" height="400" alt="image" src="https://github.com/user-attachments/assets/e151d811-8e54-4a23-962a-a411e3ea9598" />

DNS Simulation:
•	Modified hosts file:/etc/hosts
•	Added:127.0.0.1 myserver. local
<img width="723" height="342" alt="image" src="https://github.com/user-attachments/assets/ae54ce35-4f45-4bcc-9a34-103ce845f3a4" />
 
Result:
•	Website successfully accessible via: http://myserver.local
 <img width="720" height="181" alt="image" src="https://github.com/user-attachments/assets/df5dbc52-599e-44cc-87e8-dbc15f24083b" />

#### Outcome:
•	Apache successfully installed
•	Service running and accessible
•	Local web hosting environment operational
#### Windows Server – IIS Web Server
A Windows-based web server was configured using Internet Information Services (IIS) to host a local website.
#### Technologies Used:
•	Windows 10
•	IIS Web Server
•	HTML
•	Localhost hosting
### Installing IIS:
IIS was enabled using Windows Features.
 <img width="940" height="201" alt="image" src="https://github.com/user-attachments/assets/e2fad210-b8c5-4b2c-bdc9-92276f917313" />

Website Setup:
Default web directory:
IIS Windows
 <img width="511" height="291" alt="image" src="https://github.com/user-attachments/assets/d01f86e0-c4b8-4e00-871c-8cf6747d05bc" />

Created project folder:
C:\inetpub\wwwroot
<img width="940" height="222" alt="image" src="https://github.com/user-attachments/assets/e9349655-aedc-4e62-94cc-b262c7a4f0ab" />

 Running the Server:
 <img width="940" height="209" alt="image" src="https://github.com/user-attachments/assets/f42fcfba-0393-4339-8cc2-0aa70c23d291" />

#### Outcome:
•	IIS successfully configured
•	Website hosted locally and accessible via browser
#### Server Comparison
| Feature       | Apache (Linux) | IIS (Windows)       |
| ------------- | -------------- | ------------------- |
| Platform      | Linux          | Windows             |
| Configuration | Command-line   | Graphical interface |
| Flexibility   | High           | Moderate            |
| Ease of Use   | Intermediate   | User-friendly       |

	
#### Summary
The implementation of both Apache and IIS servers demonstrates my ability to manage and deploy web services across different operating systems. This reflects real-world IT environments where multiple platforms are often used together.
5. SYSTEM CHECK
A security audit was conducted on a Windows 10 system to evaluate system protection and identify vulnerabilities.
Security Checks Performed:
•	Firewall status
•	Antivirus protection			
•	System updates
•	Account security
•	Browser protection settings
Findings:
•	Firewall: Enabled
•	Antivirus: Action required 
•	System Updates: Outdated 

Actions taken:
•	Upgraded Windows 10 to 11 
 <img width="614" height="175" alt="image" src="https://github.com/user-attachments/assets/11c4735d-d01e-48c2-af4a-6209672ed5e0" />

•	Enabled PUA protection
 <img width="598" height="164" alt="image" src="https://github.com/user-attachments/assets/226fbbc4-5761-440b-bb5f-a0070813c44b" />

•	Performed antivirus scans
 <img width="614" height="358" alt="image" src="https://github.com/user-attachments/assets/5cf26763-6f27-4a03-9206-4db4a60465ab" />

#### Outcome:
•	System security posture improved
•	Key vulnerabilities addressed
## TROUBLESHOOTING 

| Issue            | Cause                          | Action Taken                                               | Result  |
| ---------------- | -----------------------------  | ---------------------------------------------------------- | ------  |
| No Internet      | Wi-Fi disabled                 | Adapter re-enabled and IP configuration renewed            |Resolved |
| Ping failure     | Firewall blocking ICMP requests| Enabled inbound ICMP rule in firewall                      |Resolved |
| Windows outdated | Outdated                       | System upgraded to Windows 11                              |Resolved |



### Network Diagram
A network topology diagram illustrating device connectivity within the local environment is attached.
 <img width="736" height="505" alt="image" src="https://github.com/user-attachments/assets/91adf5ba-2ba1-4c47-882a-9a52c81a1a88" />

## REFLECTION AND LEARNING OUTCOMES
This project helped me develop practical IT support skills across multiple areas, including system administration, networking, server management, and security.
I gained hands-on experience with:
•	Command-line tools
•	User and group management
•	Network diagnostics
•	Server deployment
•	Security auditing
I also improved my ability to troubleshoot real-world issues using a structured approach.

## CONCLUSION
This capstone project successfully demonstrates the day-to-day responsibilities of an IT Support Technician. It integrates system setup, networking, server management, security, and troubleshooting into a cohesive real-world scenario.
The project highlights the importance of technical knowledge, problem-solving skills, and proper documentation in maintaining and supporting IT systems in a professional environment.

#### Author
Jabulile Ngomane
