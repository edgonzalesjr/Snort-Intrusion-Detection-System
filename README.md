## Objective

To effectively install, configure, and utilize Snort as an Intrusion Detection System (IDS) on Ubuntu 22.04 LTS, including setting up custom and community based rules, verifying installation, and managing rule paths.

### Skills Learned

- Installation and Configuration
  - Installing Snort 3 on Ubuntu 22.04 LTS.
  - Updating shared libraries and installing prerequisites such as hyperscan.
  - Troubleshooting of installation, setup and configuration issues.
- Rule Management
  - Creating and managing custom rules for detecting specific network traffic.
  - Modifying configuration files to include and manage rule sets and paths.
  - Obtaining and integrating Oink codes for accessing additional rules.
- Service Management
  - Enabling and starting the Snort IDS service using system commands.
  - Configuring network adapter settings in Snort’s configuration file.
- Verification and Testing
  - Running Snort to monitor network traffic and confirm rule functionality.
  - Using command-line tools to filter and detect specific network traffic.
- Configuration Management
  - Modifying Snort configuration files to integrate pulledpork’s or community based rules.
  - Ensuring proper settings and paths for rule management.

### Tools Used

- Snort3: Open-source IDS/IPS tool for network traffic analysis.
- Fortigate NGFW Eval: Act as the Router and Firewall.
- Ubuntu Server: Use to host the Snort IDS and SSH server.
- Windows 10 Eval: Attacker's workstation.
- Zenmap: The official Nmap security scanner GUI.

## Lab Information

<p align="center">
<img src="https://imgur.com/8rTkja3.png" height="50%" width="50%" alt="Device Specification"/>
<br/>
<b>Network Diagram</b>
<br/>

### Lab Hosts

- FortiGate NGFW Eval
  - Router and Firewall.
- Ubuntu 22.04 LTS
  - Snort as an IDS.
- Ubuntu 22.04 LTS          
  - SSH server.
- Attacker's machine
  - Perform ping, SSH authentication and Zenmap.

## Practical Exercises

<p align="center">
<img src="https://imgur.com/xPpyFIL.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/mO0xUSv.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>Fortigate NGFW status.</b>
<br/>

<p align="center">
<img src="https://imgur.com/TAgKfKr.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/74boOf5.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>Snort IDS IP address and status.</b>
<br/>

<p align="center">
<img src="https://imgur.com/ZxKW86Y.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>SSH server IP address and status.</b>
<br/>

- Generate traffic
<p align="center">
<img src="https://imgur.com/tjUO2Li.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/pGPv4S8.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>Attacker's machine perform ping, Zenmap and SSH authentication attempts to SSH server.</b>
<br/>

- Snort IDS alert
<p align="center">
<img src="https://imgur.com/t1qHDYN.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>Ping and SSH Authentication custom alert.</b>
<br/>

<p align="center">
<img src="https://imgur.com/8IJXuEP.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>Using the pulledpork.rules to alert nmap attempt.</b>
<br/>

## Outcome

- Created and implemented custom and community based Snort rules to detect network threats.
- Managed and updated Snort configurations and rule paths effectively.
- Verified Snort’s functionality and performance in a virtual environment.
- Utilized command-line tools to filter and detect network traffic.
- Alerts were triggered by the Ping traffic, SSH authentication attempts, and Zenmap scans.

## Acknowledgements

This project combines ideas and methods from various sources, such as the installation guide by MyDFIR and my personal experience. These resources provided the fundamental information and techniques, which were then modified in light of practical uses.
 - [MyDFIR](https://github.com/MyDFIR/snort3-install-guide)
 - [Snort](https://docs.snort.org/)
 - [Fortigate NGFW Eval]()
 - [Ubuntu Server](https://ubuntu.com/download/server)
 - [Windows 10 Eval](https://www.microsoft.com/en-us/evalcenter/evaluate-windows-10-enterprise)
 - [Zenmap](https://nmap.org/zenmap/)

## Disclaimer

The sole goals of the projects and activities here are for education and ethical cybersecurity research. All work was conducted in controlled environments, such as paid cloud spaces, private labs, and online cybersecurity education platforms. Online learning and cloud tasks adhered closely to all usage guidelines. Never use these projects for improper or unlawful purposes. It is always prohibited to break into any computer system or network. Any misuse of the provided information or code is not the responsibility of the author or authors. 
